# Verification checklist

Work through this after the test steps. Do not assume it works: confirm each item.

- [ ] `show cluster info` shows one control node and the expected data nodes.
- [ ] `show cluster info health` shows healthy nodes and interfaces.
- [ ] Cluster Live Status shows all nodes in sync.
- [ ] Only one data interface type is used in the cluster.
- [ ] After a control-node failover, the main cluster IP is reachable on the new control node.
