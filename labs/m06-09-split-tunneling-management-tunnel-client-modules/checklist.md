# Verification checklist

Work through this after the test steps. Do not assume it works: confirm each item.

- [ ] Split tunnel networks or domains are correct in the group policy.
- [ ] The client route table shows only corporate networks in the tunnel.
- [ ] The management tunnel profile uses certificate authentication, and machine certificates are installed and trusted.
- [ ] There is no banner in the management tunnel group policy.
- [ ] Client modules show as configured in the group policy.
- [ ] `show vpn-sessiondb anyconnect` shows the expected sessions.
