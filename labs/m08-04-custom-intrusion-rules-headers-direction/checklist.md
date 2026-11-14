# Verification checklist

Work through this after the test steps. Do not assume it works: confirm each item.

- [ ] The engine version was checked before writing the rule.
- [ ] Header fields (action, protocol, addresses, ports, direction) match the intended traffic only.
- [ ] Message, classification and a local SID are set.
- [ ] The rule is enabled in the intrusion policy and the policy is deployed.
- [ ] A safe test triggers the event, with packet data visible in the management center.
- [ ] `->` is used unless both directions are really needed.
