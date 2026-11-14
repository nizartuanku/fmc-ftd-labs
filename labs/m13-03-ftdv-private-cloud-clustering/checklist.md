# Verification checklist

Work through this after the test steps. Do not assume it works: confirm each item.

- [ ] Same tier, version and Day 0 cluster setting on every node.
- [ ] The CCL is IPv4 over VXLAN on an isolated network; no VXLAN on data interfaces.
- [ ] `show cluster info` shows the cluster state as On with all nodes listed.
- [ ] Management uses the Management interface only.
- [ ] No VPN configuration is present on data nodes.
- [ ] Health check and interface monitoring were re-enabled after any topology change.
