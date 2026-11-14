# Verification checklist

Work through this after the test steps. Do not assume it works: confirm each item.

- [ ] `show nat detail`: the exemption rule's hits increase when traffic crosses the VPN. Zero hits means another rule matches first.
- [ ] `packet-tracer ... detailed`: the NAT phase names the identity rule and the address is unchanged.
- [ ] `show crypto ipsec sa`: encrypt and decrypt counters increase.
- [ ] `show route`: a valid route exists toward the remote subnet.
- [ ] The rule uses specific interfaces, not any.
