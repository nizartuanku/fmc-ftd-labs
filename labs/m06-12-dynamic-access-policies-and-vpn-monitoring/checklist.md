# Verification checklist

Work through this after the test steps. Do not assume it works: confirm each item.

- [ ] The Secure Firewall Posture package is uploaded (version 4.6 or later).
- [ ] DAP records have the intended AAA and endpoint criteria and actions.
- [ ] The DAP is associated with the RA VPN policy and deployed.
- [ ] A non-compliant device is denied and a compliant device connects.
- [ ] `show vpn-sessiondb anyconnect` and the user activity view match the expected results.
