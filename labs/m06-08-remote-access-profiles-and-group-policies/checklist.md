# Verification checklist

Work through this after the test steps. Do not assume it works: confirm each item.

- [ ] Profiles are bound to the internet-facing interface.
- [ ] Each profile assigns addresses from the intended source (pool, DHCP or AAA).
- [ ] The authentication server is reachable and answers.
- [ ] `show vpn-sessiondb anyconnect` shows the expected profile, group policy and address.
- [ ] Access control rules and the NAT exemption cover every pool.
- [ ] The configuration was deployed to the device.
