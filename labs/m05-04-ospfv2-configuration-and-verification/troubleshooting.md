# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| No OSPF neighbor appears | Wrong area, network statement or interface, or the device is not in routed mode | Check mode, area and the interface network |
| A neighbor is stuck below FULL | Mismatched parameters with the neighbor | Compare timers, area and authentication on both sides |
| Expected routes are missing | A summary or inter-area filter hides them | Review the summary range and filters |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
