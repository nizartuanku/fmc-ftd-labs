# Verification checklist

Work through this after the test steps. Do not assume it works: confirm each item.

- [ ] Connection events: traffic from the IPv6 client reaches the firewall.
- [ ] Packet Tracer: the intended NAT64 rule matches, not a broader rule placed earlier.
- [ ] `show nat detail` and `show xlate`: the IPv6 to IPv4 translations appear.
- [ ] `show route` on both families: routes exist toward the remote networks, and upstream routes point the mapped addresses back to the firewall.
- [ ] A packet capture of the DNS exchange shows the synthesized AAAA record reaching the client.
