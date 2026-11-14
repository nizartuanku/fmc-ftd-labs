# Verification checklist

Work through this after the test steps. Do not assume it works: confirm each item.

- [ ] The device is in routed mode; EIGRP interfaces belong to the global virtual router.
- [ ] `show eigrp neighbors`: the expected neighbor is listed on the expected interface.
- [ ] `show eigrp topology`: successor routes present for the key prefixes.
- [ ] `show route`: D / D EX entries for the expected networks.
- [ ] After a simulated failure, traffic follows the remaining path.
