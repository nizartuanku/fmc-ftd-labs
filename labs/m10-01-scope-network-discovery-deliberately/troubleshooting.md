# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| A host does not appear in the map | Its subnet is not monitored or its traffic does not cross a managed device | Check the monitored networks and the traffic path |
| Host data disappears after a deployment | Rediscovery after a discovery policy change | Plan changes for a maintenance window and wait for rediscovery |
| The map is overloaded with irrelevant hosts | Discovery covers every network the device can see | Limit monitored networks and zones |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
