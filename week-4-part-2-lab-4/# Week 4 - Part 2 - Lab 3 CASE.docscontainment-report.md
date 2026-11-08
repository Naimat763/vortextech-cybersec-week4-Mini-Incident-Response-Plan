# Week 4 - Part 2 - Lab 3
# NovaCart Containment Report

## 1. Incident
Unauthorized Customer Data Exposure

## 2. Objective
Stop unauthorized access and prevent
further customer data exposure.

## 3. Evidence Preserved
- Pre-containment access log
- Pre-containment SHA-256 hash

## 4. Containment Actions

### Action 1: Demo API Key Revocation
Revoked: demo-key-001

Verification:
HTTP 401 Unauthorized

### Action 2: Export API Restriction
The customer export endpoint was
temporarily disabled.

Verification:
HTTP 503 Service Unavailable

### Action 3: Application Availability
Health endpoint remained accessible.

Verification:
HTTP 200 OK

## 5. Evidence After Containment
- Post-containment access log
- Post-containment SHA-256 hash

## 6. Result
The simulated demo credential was rejected
and the customer export endpoint was disabled.

The mock application's health endpoint
remained available.

## 7. Important Limitations
This was a local mock API simulation.

No real customer data, API credentials,
production server or external system
was accessed.

## 8. Next Phase
Eradication:
Remove the underlying authorization weakness
and permanently fix the root cause.