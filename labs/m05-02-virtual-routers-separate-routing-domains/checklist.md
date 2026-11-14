# Verification checklist

Work through this after the test steps. Do not assume it works: confirm each item.

- [ ] The device is in routed mode.
- [ ] `show route vrf <name>`: each user-defined virtual router shows only its own connected and static routes.
- [ ] `show route`: the global virtual router does not contain the tenants' overlapping prefixes.
- [ ] Cross-domain traffic fails unless route leaking is configured on purpose.
- [ ] Access control rules were reviewed for each separated domain.
