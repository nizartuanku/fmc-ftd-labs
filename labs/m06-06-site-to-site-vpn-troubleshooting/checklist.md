# Verification checklist

Work through this after the test steps. Do not assume it works: confirm each item.

- [ ] Configuration is deployed on both peers and the peers are reachable.
- [ ] Dashboard and VPN events were reviewed before any debug.
- [ ] Debugs were filtered by peer and stopped afterwards.
- [ ] `show vpn-sessiondb l2l` shows the session.
- [ ] `show crypto ipsec sa` shows encrypt and decrypt counters increasing.
- [ ] Test traffic between the protected subnets succeeds.
