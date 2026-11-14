# Verification checklist

Work through this after the test steps. Do not assume it works: confirm each item.

- [ ] Fastpath rules match only specific, trusted endpoints, never broad subnets.
- [ ] GRE and other encapsulated traffic is handled with prefilter tunnel rules and tunnel zones.
- [ ] Connection events show which prefilter rule handled the flow.
- [ ] `packet-tracer ... detailed` shows the fastpath decision for the trusted flow and the access control rule for other flows.
- [ ] The risk of no IPS and no malware inspection on fastpathed flows is documented and accepted.
