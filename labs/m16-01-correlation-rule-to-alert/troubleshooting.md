# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| No correlation event | The policy is not active or the rule conditions do not match | Check the policy slider and compare the rule conditions with the intrusion event fields |
| Correlation event but no alert | No response assigned, or the alert target is unreachable | Check the response in the policy and the syslog or mail relay settings |
| Too many alerts | The rule has no snooze period | Add a snooze period to the rule |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
