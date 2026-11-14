# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| The flow is still inspected | The prefilter rule does not match the outer headers, or is not deployed | Check hosts, ports and tunnel conditions with packet-tracer |
| GRE traffic is not handled by an access rule | Encapsulated traffic needs prefilter tunnel rules | Create a tunnel rule in the prefilter policy |
| An attack passed unnoticed through a trusted flow | Fastpath skips IPS and malware inspection | Narrow the rule or remove Fastpath |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
