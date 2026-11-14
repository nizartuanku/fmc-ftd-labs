# Verification checklist

Work through this after the test steps. Do not assume it works: confirm each item.

- [ ] All nodes on the same tier and version, in routed mode.
- [ ] The CCL MTU is 154 bytes above the data MTU.
- [ ] Health-check firewall rules exist and the load balancer sees healthy backends.
- [ ] The management center was licensed before the cluster was added.
- [ ] `show cluster info` lists all nodes and one control node.
- [ ] No VPN configuration exists on data nodes.
