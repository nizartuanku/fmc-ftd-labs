# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| A specific static rule never matches | A broad Section 1 manual rule matches first | Move the broad rule after Auto NAT or make it more specific |
| Translations use the wrong address | Rule order or scope is different from what you assumed | Read the NAT phase in packet-tracer and `show nat detail` |
| Mapped addresses are unreachable | The device or upstream router cannot route the mapped address | Check routing for the mapped addresses |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
