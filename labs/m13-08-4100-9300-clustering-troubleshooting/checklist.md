# Verification checklist

Work through this after the test steps. Do not assume it works: confirm each item.

- [ ] All nodes show In Sync in the cluster status view.
- [ ] `show cluster info` lists one control node and every expected data node.
- [ ] `show cluster info health` shows healthy units and interfaces.
- [ ] `show running-config cluster` shows the expected CCL interface and MTU.
- [ ] `show interface <CCL_INTERFACE>` shows no growing input errors or drops.
- [ ] `ping <CCL_IP> size <CCL_MTU> repeat 2` succeeds to each peer.
