# Verification checklist

Work through this after the test steps. Do not assume it works: confirm each item.

- [ ] Secure Client on the endpoint shows connected and an address from the pool.
- [ ] `show vpn-sessiondb anyconnect` lists the user.
- [ ] A ping or app test to the internal server works.
- [ ] The access control rule for the VPN pool is hit.
- [ ] `show nat detail` shows the identity NAT rule hit counts increasing.
- [ ] Internal names resolve through the group policy DNS.
