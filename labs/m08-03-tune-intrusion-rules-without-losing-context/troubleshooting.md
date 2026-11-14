# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| Other hosts also stopped generating events | A threshold or a disabled rule was used instead of a scoped suppression | Use a suppression for the scanner address only |
| The scanner is still noisy after the change | The policy was not deployed or the wrong rule or policy was edited | Deploy and check the SID and the policy |
| Nobody remembers why a rule was tuned | No comment or change record | Record the reason when you tune |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
