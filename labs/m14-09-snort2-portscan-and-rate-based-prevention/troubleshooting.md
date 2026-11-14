# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| No portscan events appear | The GID 122 rules are not enabled, or stream preprocessing is off | Enable the rules and TCP/UDP stream processing |
| Too many false positives | Medium sensitivity on busy hosts such as NAT devices or proxies | Use Watch IP and Ignore Scanners or lower the sensitivity |
| Slow scans are missed | Low sensitivity detects only negative responses | Use High with tuning |
| Legitimate users are dropped | A rate threshold was set without a baseline | Measure the baseline and raise the threshold |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
