# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| The conversion option is missing or fails | Unsupported model or version, the device is a 3105, or it is not registered as standalone | Check the model, version and registration state first |
| The device is unreachable after conversion | Manager access relied on DHCP or a data interface, which do not survive the conversion | Use the dedicated Management interface with a static IP and keep console access ready |
| A data-sharing interface is rejected | It is being used for a bridge group, inline set, passive interface or failover link | Use a normal data interface for those roles |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
