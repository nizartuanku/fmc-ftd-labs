# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| Modbus rules never fire | The preprocessor port differs from the PLC port, so the traffic is generic TCP | Set the preprocessor port to the PLC port |
| The PLC link drops after a policy push | The Snort restart during deployment interrupted traffic | Check the Snort Fail Open settings and deploy in a maintenance window |
| No N flag in show conn | The traffic was not inspected by Snort | Check the access control rule, prefilter and the NAP assignment |
| Settings are missing | The device runs Snort 3 | These settings are for Snort 2 |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
