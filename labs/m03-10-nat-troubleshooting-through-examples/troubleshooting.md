# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| Every external connection is dropped | A broader NAT rule matched first, so the destination was not translated to the real server | Compare translate hits and reorder the rules |
| You keep editing access rules with no change | The packet never matches the intended NAT rule | Fix NAT order before touching access control |
| A service behind PAT is unreachable | PAT creates translations only for outbound connections | Use a static mapping |
| Changes seem to have no effect | The latest policy was not deployed or is out of date | Check deployment status for the device |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
