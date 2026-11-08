# Week 4 - Part 2 - Lab 6
# NovaCart Post-Incident Review

## 1. Incident Summary

Company: NovaCart Online
Incident: Unauthorized Customer Data Exposure
Incident Type: API Authorization Failure
Priority: High (Scenario Classification)

## 2. What Happened?

A normal customer account accessed an administrative
customer-export API because server-side function
authorization was missing.

The simulated API logs recorded two requests,
each returning 4800 customer records.

## 3. Root Cause

Missing server-side authorization checks on
the administrative customer-export function.

## 4. Detection Review

SIEM detected unusual customer export activity.

First suspicious request: 10:02:11 UTC
SIEM alert: 10:08:00 UTC

Simulated detection interval: 5 minutes 49 seconds.

This is a training-log calculation, not a
production MTTD measurement.

## 5. What Went Well?

- API Gateway logs contained request details.
- SIEM generated a high-severity alert.
- Investigation evidence was preserved.
- SHA-256 hashes were generated.
- Demo credentials were revoked.
- Authorization weakness was fixed.
- Customer and Admin tests were performed.
- Service was restored after security checks.

## 6. What Could Be Improved?

- Detect unauthorized role access earlier.
- Add authorization tests to every admin API.
- Improve SIEM correlation and alert tuning.
- Maintain complete incident timestamps.
- Improve evidence collection procedures.
- Conduct regular incident-response exercises.

## 7. Lessons Learned

1. Every sensitive API must enforce
   server-side authorization.

2. SIEM must identify unusual administrative
   API access from customer accounts.

3. Logs should include request IDs, verified
   user roles, API paths and response status.

4. Incident response actions should have
   named owners and clear procedures.

5. Backup restoration and security checks
   should be tested regularly.

## 8. Unknown Information

- External customer-data download is unconfirmed.
- Misuse of the exposed records is unconfirmed.
- Unique affected customer count is unknown.
- Full database audit evidence is unavailable.

## 9. Review Approach

This review is blameless.
It focuses on improving security controls,
processes, monitoring and team readiness,
not blaming an individual.

## 10. Training Scope

All incidents and records are fictional.
No real company or customer data was involved.