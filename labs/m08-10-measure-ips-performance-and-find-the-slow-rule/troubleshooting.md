# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| Latency rises after a new custom rule | The rule relies on PCRE alone | Add a strong content match first |
| Traffic skipped inspection during a peak | Packet latency thresholding stopped inspecting slow packets | Fix the slow rule and review the threshold |
| Traffic blipped after deploying | The deployment restarted the Snort process | Read the deployment warnings and plan the window |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
