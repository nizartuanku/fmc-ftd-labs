# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| The custom NAP is never used | No network analysis rule matches the traffic, so the default NAP applies | Check the rule's zones or networks and its order |
| Settings you expected are missing | The inspection engine (Snort 2 or Snort 3) does not offer them | Check the engine version first |
| A deploy changes more than you expected | No comparison or preview was reviewed | Compare revisions and use the deployment preview |
| Intrusion events never show early in a connection | The pre-identification intrusion policy is not set as intended | Review the policy in Advanced settings |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
