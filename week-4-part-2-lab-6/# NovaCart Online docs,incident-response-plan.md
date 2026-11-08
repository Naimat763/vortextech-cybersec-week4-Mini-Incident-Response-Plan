# NovaCart Online
# Mini Incident Response Plan

Training Institute: Vortex Tech Academy
Program: Cyber Security Internship
Scenario: Hypothetical Customer Data Exposure

---

## 1. Executive Summary

NovaCart Online experienced a simulated
customer-data exposure incident caused by
missing server-side authorization on an
administrative API endpoint.

## 2. Company and Incident Scenario

Company: NovaCart Online
Business: E-commerce

Affected Component:
/api/v1/admin/customers/export

Root Cause:
Missing server-side function-level authorization.

Data at Risk:
Names, emails, phone numbers, shipping addresses
and order history.

External misuse remains unconfirmed.

## 3. Incident Response Framework

The plan follows the six phases used in
the Vortex Week 4 assignment:

1. Preparation
2. Detection and Analysis
3. Containment
4. Eradication
5. Recovery
6. Lessons Learned

## 4. Preparation

- Identify critical systems and assets.
- Define incident-response team roles.
- Maintain SIEM and API monitoring.
- Verify backups and restoration procedures.
- Maintain escalation contacts and playbooks.

## 5. Detection and Analysis

- Detect unusual API export activity.
- Validate SIEM alerts.
- Review API Gateway and database logs.
- Identify affected accounts and endpoints.
- Preserve evidence and build an incident timeline.

## 6. Containment

- Revoke compromised credentials.
- Restrict affected API endpoints.
- Preserve original logs.
- Verify that unauthorized access has stopped.

## 7. Eradication

- Remove the authorization weakness.
- Enforce server-side role verification.
- Remove malicious access.
- Test Customer and Admin permissions.

## 8. Recovery

- Verify secure configurations and backups.
- Test application functionality.
- Restore approved services.
- Monitor post-recovery activity.

## 9. Lessons Learned

- Review the incident and timeline.
- Identify root causes and response gaps.
- Assign owners to improvement actions.
- Update security procedures and playbooks.

## 10. Communication Plan

- Immediately escalate major incidents
  to incident leadership.
- Engage Legal and Privacy teams early.
- Coordinate technical responders.
- Notify affected customers and regulators
  according to applicable requirements.
- Use approved communication channels.

## 11. Preventive Measures

1. Enforce server-side API authorization.
2. Add automated API authorization tests.
3. Improve SIEM monitoring for unusual exports.

## 12. Conclusion

This incident-response plan demonstrates how
an organization can prepare for, detect,
contain, eradicate, recover from and learn
from a hypothetical customer-data exposure.

## 13. Scope and Limitations

This is a fictional training scenario.
No real production incident or customer data
was involved.

All practical exercises were conducted
within controlled local environments.