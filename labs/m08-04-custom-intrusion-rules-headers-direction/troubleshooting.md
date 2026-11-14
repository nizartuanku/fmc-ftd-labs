# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| The rule never fires | It is saved but not enabled in the intrusion policy, or the policy was not deployed | Enable it with the normal state or action and deploy |
| Too many false positives | The header is too broad (any ports or both directions) | Narrow the ports and use the one-way direction |
| The event has no packet data | Transfer Packets is disabled | Enable it in the device's general settings |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
