# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| A blocked indicator still connects | The address is on the Do Not Block list, publishing is paused or the traffic is trusted or bypasses inspection | Check each of those and the observable's own action |
| The action differs from what you set on the source | The observable carries its own action | Check the observable's action |
| No incident appears | The Do Not Block list matched first, or publishing has not completed | Wait for publishing and check the Do Not Block list |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
