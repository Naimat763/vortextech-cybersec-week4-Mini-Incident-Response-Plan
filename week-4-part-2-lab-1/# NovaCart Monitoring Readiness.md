# NovaCart Monitoring Readiness

## Monitoring Sources

1. API Gateway Logs
2. Database Audit Logs
3. SIEM Security Alerts
4. Firewall / WAF Logs
5. Server Authentication Logs

## Example Alert Rule

IF:
- User role = customer
- API endpoint = admin customer export
- Response status = 200

THEN:
- Generate a high-priority alert.
- Notify SOC Analyst.
- Start investigation.

## Required Log Fields

- Timestamp
- Request ID
- User ID / Role
- Source IP
- API endpoint
- HTTP response status
- Records returned

## Security Note

Never log passwords, authentication tokens,
or unnecessary sensitive customer information.

## Local Practical

Ubuntu SSH logs checked using journalctl.
NovaCart SIEM is a hypothetical design,
not an installed SIEM deployment.