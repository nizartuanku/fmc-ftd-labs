# Verification checklist

Work through this after the test steps. Do not assume it works: confirm each item.

- [ ] The device is in routed mode; multicast interfaces are routed, not BVI members.
- [ ] `show igmp groups`: the test group appears on the receiver interface.
- [ ] `show pim neighbor`: PIM neighbors present on the source-facing side.
- [ ] `show mroute`: an entry exists for the group with the expected incoming and outgoing interfaces.
- [ ] The access control policy allows the stream.
