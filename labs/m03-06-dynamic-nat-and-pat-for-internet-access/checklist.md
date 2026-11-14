# Verification checklist

Work through this after the test steps. Do not assume it works: confirm each item.

- [ ] `show nat detail`: your rule's translate hits increase while users browse.
- [ ] `show xlate`: many inside hosts share the public address, each with its own port.
- [ ] If the mapped address is not the outside interface address, the upstream router has a route to it pointing at the firewall.
- [ ] The rule names the real inside and outside interfaces, not any.
- [ ] `packet-tracer` shows the expected translation.
