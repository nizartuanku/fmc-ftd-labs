# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| All traffic still goes through the tunnel | The client was not reconnected, or the split setting is not in the active group policy | Reconnect and check the group policy bound to the profile |
| A domain exclusion has no effect | The custom attribute is missing or misspelled | Re-check the dynamic split custom attribute in the group policy |
| The management tunnel never comes up before login | The machine certificate is missing, invalid or not trusted | Check the machine certificate store and that the CA is trusted by the threat defense |
| The management tunnel fails with a banner configured | A banner is set in the management group policy | Remove the banner |
| A client module does not load | The module profile was not uploaded or not attached | Upload it as a Secure Client file and attach it in the group policy |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
