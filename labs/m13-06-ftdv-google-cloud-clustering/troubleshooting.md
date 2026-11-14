# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| Backends show unhealthy | No firewall rule allows health-check traffic | Add the health-check firewall rules |
| Nodes will not form a cluster | Mixed tier or version, or the Day 0 script is wrong | Rebuild from the guide's Day 0 sample and match tier and version |
| Large CCL packets are dropped | The CCL MTU is not 154 bytes above data on the cloud network | Fix the MTUs |
| Management or VPN on a data node fails | Neither is supported on data nodes or data interfaces | Use the Management interface; VPN on the control node only |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
