# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| Events did not drop after the change | The policy was not deployed or the threshold is disabled | Deploy and check the setting |
| A second target's events are missing | Track By is set to source and the source count is already reached | Check the Track By choice |
| Attacks seem to pass after tuning | Only logging is limited; check whether the rule still drops | Verify with a drop test |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
