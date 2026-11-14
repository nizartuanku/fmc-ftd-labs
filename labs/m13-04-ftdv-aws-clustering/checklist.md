# Verification checklist

Work through this after the test steps. Do not assume it works: confirm each item.

- [ ] All nodes are FTDv20 or higher and on the same tier.
- [ ] All CCL interfaces are in one subnet.
- [ ] The management center was licensed before registration.
- [ ] Every node shows In Sync in the Cluster Status dialog.
- [ ] `show cluster info` on a node lists all nodes and one control node.
- [ ] GWLB target failover is set to rebalance (threat defense 7.4.1 or later).
