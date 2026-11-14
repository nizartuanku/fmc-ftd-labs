# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| The lookup returns the real address | The DNS policy is not linked or not deployed, or the query does not pass through the firewall | Link the policy, deploy and check the resolver path |
| No hits appear in events | The rule condition does not match the zone or the list | Check the source zone and the DNS list contents |
| A threat still connects | The malware uses a hard-coded address, not DNS | Use IP-based Security Intelligence and access control |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
