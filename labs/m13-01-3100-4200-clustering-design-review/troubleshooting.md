# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| A node will not join the cluster | Hardware, version, mode, domain or group differs, or a deployment is pending | Compare the node table from Part 1 and clear pending deployments |
| Large CCL packets are dropped | The switch MTU on the CCL path is lower than the CCL MTU | Raise the switch port MTU to at least the CCL MTU |
| Odd behavior after a time change | Nodes use different or manually set time | Point all nodes to the same NTP source |
| Interface configuration is rejected | Spanned EtherChannel and Individual interfaces are mixed | Use one data interface type everywhere |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
