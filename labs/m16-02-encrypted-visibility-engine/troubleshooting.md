# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| EVE columns are empty | Snort 2, no IPS license or logging disabled | Check the inspection engine, the license and the rule logging |
| Traffic is not classified | The traffic is tunnelled or encapsulated | EVE cannot see inside encapsulated traffic |
| A legitimate tool is blocked | Its fingerprint scores above the threshold | Add an EVE exception rule for the process or destination |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
