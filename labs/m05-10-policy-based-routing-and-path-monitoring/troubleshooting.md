# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| The test flow ignores PBR | The ACL does not match, or PBR is not applied on the ingress interface | Check the ACL and the ingress interface with packet-tracer |
| Traffic is dropped after enabling PBR | uRPF is still enabled on the interface | Disable uRPF where PBR is used |
| Metric-based ordering has no effect | Path monitoring is not enabled on the egress interfaces | Enable path monitoring on each egress interface |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
