# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| A node stays unregistered | Registration did not complete | Use Reconcile All in the Cluster Status dialog |
| Data units leave and rejoin after licensing | The cluster was added while the management center was in evaluation mode | License the management center first |
| Sessions drop when a node fails | GWLB target failover is no_rebalance, so existing flows stay on the failed target | Set rebalance where supported |
| The template fails with FTDv5 or FTDv10 | These tiers do not support AWS GWLB | Use FTDv20 or higher |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
