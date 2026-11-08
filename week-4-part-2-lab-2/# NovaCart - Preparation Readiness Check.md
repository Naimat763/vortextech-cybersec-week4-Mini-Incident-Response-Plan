# Week 4 - Part 2 - Lab 2
# Detection and Analysis Report

## 1. Incident Overview
Company: NovaCart Online
Incident: Customer Data Exposure
Environment: Fictional Training Scenario

## 2. Detection Source
SIEM Alert: Large_Customer_Export
Severity: High (Sample Alert)

## 3. Suspicious Activity
Account: CUST-104
Role: customer
Source IP: 198.51.100.24
Affected API: /api/v1/admin/customers/export
HTTP Status: 200
Records: 4800 per logged request

## 4. Investigation Findings
- Two suspicious export requests were identified.
- The account role was customer.
- The endpoint was intended for admin functions.
- The simulated API logs recorded 4800 returned records.
- SIEM generated a high-severity alert.

## 5. Scope of Investigation
Affected component: Customer Export API
Affected account: CUST-104
Potentially affected data:
- Names
- Email addresses
- Phone numbers
- Shipping addresses
- Order history

## 6. Timeline
10:00 UTC - Normal catalogue request
10:01 UTC - Normal order request
10:02 UTC - Suspicious admin API access
10:03 UTC - Repeated export request
10:08 UTC - SIEM alert generated

## 7. Initial Classification
Incident type: Suspected unauthorized data exposure
Priority: High (Provisional)
Root cause hypothesis:
Missing server-side function-level authorization.

## 8. Unknown Information
- External download is not confirmed.
- Actual number of unique records is unknown.
- Database audit logs have not been reviewed.
- Whether other accounts were affected is unknown.

## 9. Evidence
evidence/api-gateway-sample.log
evidence/SHA256SUMS.txt

## 10. Training Scope
All events are synthetic and created for a
controlled local incident-response exercise.
No real customer records were accessed.

## 11. Next Action
Preserve evidence and proceed to the
Containment phase under the incident response plan.