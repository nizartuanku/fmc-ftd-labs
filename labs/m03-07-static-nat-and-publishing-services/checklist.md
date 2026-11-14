# Verification checklist

Work through this after the test steps. Do not assume it works: confirm each item.

- [ ] Packet tracer shows the un-NAT to the real IP, then your access rule matching.
- [ ] `show nat detail`: hits increase on the static rule.
- [ ] `show xlate`: a static translation exists between the real and mapped addresses.
- [ ] Connection events show the session allowed by the intended rule.
- [ ] Upstream routing delivers the mapped address to the firewall.
