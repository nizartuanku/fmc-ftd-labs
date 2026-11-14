# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| Legitimate traffic is dropped | Checksum verification is set to drop and the traffic has offloaded or invalid checksums | Review the checksum action per protocol |
| Expected defrag options have no effect | Policy, Detect Anomalies and Overlap Limit are ignored on routed and transparent interfaces | Check the interface mode |
| Fragments are dropped at the device | The platform Fragment Settings limits were exceeded | Review Chain, Size and Timeout |
| No normalization happens | Inline Mode is off or the device is not inline | Enable Inline Mode and deploy inline |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
