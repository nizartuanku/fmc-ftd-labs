# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| Everything stops after the first deployment | The default action is Block all traffic and no rules cover the needed subnets or DNS | Add the rules first or set the default action deliberately |
| A local Allow does not override a base Block | Base Mandatory rules are evaluated first and locked | Change the base policy if the exception is legitimate |
| Policy assignment fails | A required license or a supported feature is missing on the device | Check licenses and model support |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
