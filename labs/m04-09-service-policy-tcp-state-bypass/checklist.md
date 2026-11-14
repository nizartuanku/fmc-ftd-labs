# Verification checklist

Work through this after the test steps. Do not assume it works: confirm each item.

- [ ] The extended access list matches only the affected endpoints.
- [ ] The rule is global when return traffic can arrive on a different interface.
- [ ] `show asp drop`: the TCP state drop counters stop increasing for the flow.
- [ ] `show service-policy` shows the TCP state bypass setting applied.
- [ ] No conflicting FlexConfig policy maps exist on the same interfaces.
- [ ] A follow-up task exists to make the routing symmetric.
