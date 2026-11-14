# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| The example commands fail on the device | The hardware or software does not match the example | Pick an example for your model and version |
| Deployment shows an error after upgrade | The same policy is configured in FlexConfig and in the GUI | Remove the migrated objects from the FlexConfig policy copy |
| Variables are empty in the preview | The text object or variable mapping is missing | Fix the mapping and preview again |
| Everything rolled back | A single FlexConfig error rolls back the deployment attempt | Fix the rejected line named in the transcript |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
