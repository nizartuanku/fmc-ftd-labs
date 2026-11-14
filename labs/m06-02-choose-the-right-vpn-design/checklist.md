# Verification checklist

Work through this after the test steps. Do not assume it works: confirm each item.

- [ ] Licensing allows strong encryption.
- [ ] VPN headends run in routed mode.
- [ ] Remote access VPN is not planned on clustered devices.
- [ ] The team knows that site-to-site VPN in a cluster runs on the control node and drops on control-node failover.
- [ ] Tunnel status is green in the management center and `show crypto ipsec sa` shows encrypt and decrypt counters increasing.
- [ ] Routing (static or dynamic) sends the protected traffic into the VPN.
