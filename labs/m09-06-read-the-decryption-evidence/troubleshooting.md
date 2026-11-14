# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| No recent events for a device | The management connection is down | Check the management connection; the device still enforces policy |
| One application breaks only when decrypted | It pins its certificate | Add a Do Not Decrypt exception |
| OVER_SUBSCRIBED flags appear | Decryption demand exceeds platform capacity | Add Do Not Decrypt rules for lower-priority traffic or use a larger device |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
