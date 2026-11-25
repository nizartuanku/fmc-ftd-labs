# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| Ingress capture is empty | Traffic does not reach the interface or the match is wrong | Check routing upstream and the capture match |
| Packet tracer allows but real traffic drops | The virtual packet does not match real traffic | Use a capture with trace on real packets |
| Engine debug shows nothing | The flow is fastpathed or blocked before Snort | Check prefilter rules and the LINA phases in the trace |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
