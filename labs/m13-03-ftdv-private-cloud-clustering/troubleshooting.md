# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| Nodes will not form a cluster | Different tiers or versions, a pending deployment, or the Day 0 cluster setting is missing | Redeploy the node with the Day 0 cluster setting and match tier and version |
| Large CCL packets are dropped | The CCL MTU path is too small (needs 154 bytes above the highest data MTU) | Raise the MTU on the CCL network |
| VPN configuration is rejected on a data node | Site-to-site VPN is supported on the control node only | Configure VPN on the control node only |
| Management from a data interface does not work | Only the Management interface is supported for management | Use the Management interface |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
