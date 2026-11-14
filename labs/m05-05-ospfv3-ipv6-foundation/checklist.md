# Verification checklist

Work through this after the test steps. Do not assume it works: confirm each item.

- [ ] `show ipv6 interface brief`: both link-local and global addresses present, interface up.
- [ ] No duplicate-address messages (syslog 325002) for the interface.
- [ ] `show ipv6 ospf neighbor`: neighbor reaches FULL.
- [ ] `show ipv6 route`: OSPFv3-learned prefixes present.
- [ ] Bridge-group (transparent) designs: ICMPv6 types 135 and 136 are permitted.
