# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| No port scan events appear | The device uses Snort 2, the mode is Disable, or the sensitivity is too low for a slow scan | Check the engine, the mode and the sensitivity |
| An internal scanner keeps getting blocked | It is not on the exclude list | Add it to the exclude list |
| A blocked host stays blocked | It remains shunned for the configured duration | Release it with the CLI clear command |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
