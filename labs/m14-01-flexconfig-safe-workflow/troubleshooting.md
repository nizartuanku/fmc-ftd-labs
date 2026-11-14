# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| The whole deployment is rolled back | A FlexConfig command was rejected by the device | Read the transcript, fix or remove the command and deploy again |
| The command is not on the device | The policy targets the wrong device or the object is not in the policy | Check the policy targets and Preview Config |
| The command remains after unassigning the policy | Unassigning does not necessarily remove deployed commands | Deploy the negate command |
| A feature seems to be configured twice | The same feature is managed in the GUI and in FlexConfig | Use only the managed feature |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
