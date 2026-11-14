# Verification checklist

Work through this after the test steps. Do not assume it works: confirm each item.

- [ ] Hardware mixing follows the native or container rules; no 4100 and 9300 in one cluster.
- [ ] The CCL runs through a switch with an MTU at least 100 bytes above data.
- [ ] On a 9300, all 3 modules are part of the cluster.
- [ ] `show cluster info` lists every unit and one control node.
- [ ] `show cluster info health` shows healthy units and interfaces.
- [ ] Throughput planning uses about 80 percent of combined capacity.
