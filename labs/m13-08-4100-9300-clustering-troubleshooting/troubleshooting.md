# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| Small pings work but the large ping fails | A switch on the CCL path has a smaller MTU than the CCL | Raise the MTU on every CCL switch port |
| A node shows clustering is disabled | It was ejected from the cluster, often after CCL or health problems | Check the CCL path and node health, then rejoin the node |
| Throughput drops by about half with no alarm | A data node left the cluster and its load moved to the others | Check Cluster Live Status and the health dashboard first |
| Input errors grow on the CCL interface | Link or MTU problem | Inspect the interface counters and the switch ports |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
