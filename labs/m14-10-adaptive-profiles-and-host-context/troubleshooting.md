# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| No change in inspection after enabling | Network discovery has no data for the host | Fix the discovery policy or import host data |
| Profile updates do not seem to apply | Enable Profile Updates is not selected, or the Networks field excludes the host | Select it and check the Networks field |
| Stale decisions about a host | Host data is old after an OS or role change | Keep discovery running and shorten the update interval sensibly |
| Rules were enabled or disabled unexpectedly | Recommended rules were applied, which is separate from profile updates | Review recommended-rule changes per intrusion policy |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
