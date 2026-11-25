# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| No events in the cloud | EMBLEM is on, or syslog does not reach the SEC | Turn EMBLEM off and check reachability to the SEC port |
| Events missing device names | Device ID not enabled | Enable the device ID in syslog settings |
| Duplicate events | Both syslog and direct paths are on | Use one path per event type |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
