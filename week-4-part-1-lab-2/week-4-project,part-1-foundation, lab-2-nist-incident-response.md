# Week 4 - Part 1 - Lab 2
# NovaCart Online - Company Breach Scenario

## 1. Company Overview
Company: NovaCart Online
Business: E-commerce
Customers: 20,000 (Hypothetical)
Employees: 80 (Hypothetical)

## 2. Incident
Unauthorized Customer Data Exposure

## 3. Affected Component
Admin Customer Export API

Endpoint:
/api/v1/admin/customers/export

## 4. Root Cause
Missing server-side role-based authorization
allowed a normal customer account to access
an administrative API function.

## 5. Detection
A SIEM alert identified unusual customer-data
export activity from a normal customer account.

## 6. Evidence
- Customer role accessed admin export API.
- HTTP response status was 200.
- API logs recorded 4,800 returned records.
- SIEM generated a high-severity alert.

## 7. Data at Risk
- Customer names
- Email addresses
- Phone numbers
- Shipping addresses
- Order history

Payment card details and passwords are not
included in this scenario.

## 8. Incident Timeline
10:00 UTC - Normal catalogue request
10:01 UTC - Normal order request
10:02 UTC - Suspicious admin API access
10:03 UTC - Second large export request
10:08 UTC - SIEM alert generated

## 9. Potential Impact
- Customer privacy violation
- Phishing risk
- Fraud attempts
- Reputation damage
- Possible regulatory obligations

## 10. Unknown Information
External download or misuse of records
has not been confirmed.

## 11. Classification
OWASP API5:2023 - Broken Function Level Authorization
Related general category:
OWASP A01:2025 - Broken Access Control

## 12. Training Scope
All log entries are fictional and generated
for a controlled local training exercise.
No real customer data was accessed.