# Week 4 - Part 2 - Lab 5
# NovaCart Recovery Report

## 1. Incident
Unauthorized Customer Data Exposure

## 2. Recovery Objective
Restore the secure customer export service
without reintroducing the authorization weakness.

## 3. Pre-Recovery Checks
- Secure code syntax verified.
- Original containment state verified.
- Revoked key status preserved.
- Customer authorization tested.
- Admin access remained restricted before restoration.

## 4. Backup Verification
- Synthetic backup created.
- SHA-256 hash calculated.
- Restored copy compared with backup.
- File integrity test passed.

## 5. Recovery Action
- Secure mock API started.
- Export endpoint re-enabled.
- Old revoked key remained revoked.

## 6. Post-Recovery Tests

Admin: HTTP 200 - PASS
Customer: HTTP 403 - PASS
Revoked Key: HTTP 401 - PASS
Health Check: HTTP 200 - PASS

## 7. Post-Recovery Monitoring
- Secure API access logs reviewed.
- Unauthorized customer success pattern not found.
- Authorized admin activity verified.

## 8. Limitations
This was a local mock API exercise.
No production service or real customer database
was restored.

## 9. Recovery Outcome
The simulated service was restored while
server-side authorization and revoked-key
controls remained effective.

## 10. Next Phase
Lessons Learned and post-incident review.