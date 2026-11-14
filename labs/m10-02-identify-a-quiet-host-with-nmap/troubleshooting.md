# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| The scan has no effect on the host profile | The instance has no target, or a higher-ranked source overrides it | Add a target and check the source ranking |
| A custom fingerprint is never used | It was created but not activated | Activate it |
| Passive and active data disagree | Identity conflict settings decide which wins | Review the identity conflict settings |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
