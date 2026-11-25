# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| Authorization fails | Wrong region or tenant, or no outbound HTTPS | Check the region, tenant and firewall rules for 443 |
| Duplicate events | Both direct and syslog sending are on | Disable one path |
| Events in SSE but not XDR | Events are not promoted | Check automatic promotion in SSE |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
