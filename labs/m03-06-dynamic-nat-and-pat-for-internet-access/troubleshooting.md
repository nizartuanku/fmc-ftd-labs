# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| Users cannot reach the internet | Private addresses are not translated, or the rule uses the wrong interface | Check the rule's interfaces and hit counters |
| Hits increase but replies never arrive | The upstream router has no route to a mapped address that is not the interface address | Add the route toward the firewall |
| The pool runs out | Dynamic NAT (not PAT) has too few public addresses | Use dynamic PAT |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
