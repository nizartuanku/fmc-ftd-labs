# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| A new Block rule never triggers | A broader Allow rule above it matches first | Move the specific rule above the broad one |
| A user condition never matches | No identity policy is associated with the access control policy | Associate an identity policy |
| Malicious traffic gets through on port 443 | The rule is port-based, not application-based | Use application conditions |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
