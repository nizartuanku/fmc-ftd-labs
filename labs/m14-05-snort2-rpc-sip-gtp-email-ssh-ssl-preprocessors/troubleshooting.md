# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| Malformed packets are only alerted, not dropped | The device is passive, Inline Mode is off, or the rules are not set to drop | Use an inline deployment, enable Inline Mode and set the rules to drop |
| Traffic passes uninspected during a Snort failure | The Snort Fail Open Down default lets traffic pass | Decide the Down and Busy options per inline set |
| You expect to see inside an SSH or TLS session | The SSH and SSL preprocessors do not decrypt | Use a decryption policy |
| Settings missing on the device | The device runs Snort 3 | These NAP settings are for Snort 2 |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
