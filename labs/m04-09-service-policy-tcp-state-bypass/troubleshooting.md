# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| Sessions still drop after the change | The access list does not match both directions or the rule is not global | Check the list and the rule scope |
| Deployment fails after adding the rule | A manual FlexConfig policy map conflicts with the native service policy | Remove the conflicting FlexConfig object |
| Other traffic lost TCP state checking | The access list is too broad | Narrow it to the affected endpoints |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
