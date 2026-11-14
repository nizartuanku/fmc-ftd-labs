# Verification checklist

Work through this after the test steps. Do not assume it works: confirm each item.

- [ ] Same model, interfaces, version and firewall mode on all nodes.
- [ ] CCL switch ports carry the CCL MTU (100 bytes above the highest data MTU).
- [ ] The CCL uses a switch, not a back-to-back cable.
- [ ] One data interface type is used across the cluster.
- [ ] After forming, `show cluster info` lists every node with the expected role.
- [ ] `show cluster history` shows no MTU-check failures.
