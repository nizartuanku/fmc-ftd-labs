# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| The service is unreachable from outside | The access rule uses the mapped address as destination | Use the real address in the access rule |
| Traffic never reaches the firewall | Upstream routing does not deliver the mapped address | Add the route toward the firewall |
| An inside host cannot publish a service with PAT | PAT ports are assigned on demand | Use static NAT |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
