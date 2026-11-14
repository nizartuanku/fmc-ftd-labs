# Verification checklist

Work through this after the test steps. Do not assume it works: confirm each item.

- [ ] The profile uses at least two factors (certificate and AAA, or MFA).
- [ ] Devices without a valid certificate are rejected.
- [ ] The RADIUS timeout is at least 60 seconds for MFA.
- [ ] Every group policy the RADIUS server can return is in the RA VPN policy and deployed.
- [ ] `show vpn-sessiondb anyconnect` shows the expected group policy per user.
- [ ] Accounting records reach the RADIUS server and failed logins appear in the logs.
