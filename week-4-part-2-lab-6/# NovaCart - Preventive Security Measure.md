# NovaCart - Preventive Security Measures

## Root Cause
Missing server-side authorization on the
administrative customer export API.

## Measure 1 - Server-Side Authorization

Action:
Enforce role-based authorization on every
sensitive API endpoint.

Owner:
API Engineering Lead.

Success Criteria:
Customer receives HTTP 403.
Authorized Admin receives permitted access.

## Measure 2 - Automated API Security Testing

Action:
Add role-based authorization tests to CI/CD.

Owner:
Application Security / QA Lead.

Success Criteria:
Customer, Admin and unauthenticated
access tests pass before release.

## Measure 3 - SIEM Monitoring

Action:
Create alerts for customer-role access to
administrative endpoints and unusual exports.

Owner:
SOC Detection Engineer.

Success Criteria:
A simulated unauthorized access event
generates a validated SIEM alert.

## Conclusion

These controls reduce the likelihood of
unauthorized administrative API access
and improve detection capability.