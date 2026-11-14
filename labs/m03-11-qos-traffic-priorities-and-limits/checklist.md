# Verification checklist

Work through this after the test steps. Do not assume it works: confirm each item.

- [ ] The policy is assigned and deployed to the right device (one QoS policy per device).
- [ ] The rule is on a routed interface, not a VTI or site-to-site VPN path.
- [ ] The traffic is allowed or trusted by access control, not fastpathed by a prefilter rule.
- [ ] The specific rule sits above broader rules (first match wins), and the device stays under 255 QoS rules.
- [ ] Connection events show the dropped traffic and which QoS configuration limited it.
