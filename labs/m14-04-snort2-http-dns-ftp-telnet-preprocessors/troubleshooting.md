# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| A correct-looking rule never fires | It matches the encoded form but the buffer holds the normalized form | Write the rule for the normalized buffer or use a raw buffer on purpose |
| Your NAP changes have no effect | They were not committed, assigned or deployed | Commit, assign the NAP and deploy |
| Nothing is normalized or dropped | Inline Mode is off or the device is deployed passively | Enable Inline Mode and deploy inline |
| Settings do not exist on the device | The device runs Snort 3 | These settings are for Snort 2 |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
