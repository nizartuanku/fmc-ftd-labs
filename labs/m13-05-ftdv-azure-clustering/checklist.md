# Verification checklist

Work through this after the test steps. Do not assume it works: confirm each item.

- [ ] All nodes on the same tier, version and interfaces.
- [ ] The CCL range contains only the addresses you need (16 at most).
- [ ] The management center was licensed before the cluster was added.
- [ ] `show cluster info` shows all nodes and one control node.
- [ ] The storage account's outqueue logs show the Function App's processing.
- [ ] No VPN configuration exists on data nodes.
