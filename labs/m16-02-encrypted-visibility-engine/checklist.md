# Verification checklist

Work through this after the test steps. Do not assume it works: confirm each item.

- [ ] The device runs Snort 3 and the deployment shows no license warning.
- [ ] Test traffic is logged.
- [ ] EVE columns show a process name for each tool.
- [ ] No legitimate application was blocked; any false block is handled with an exception rule, not a lower global threshold.
