# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| The tunnel is up but nothing passes | A broader NAT rule translates the traffic before the VPN | Add an identity NAT rule above it |
| The exemption has zero hits | Another rule above it matches first | Move the exemption above the broader rule |
| Internet access breaks after adding the exemption | The exemption uses any interfaces and exempts unrelated traffic | Use specific source and destination interfaces |
| Encrypt counters stay at zero | No route or interesting traffic toward the remote subnet | Check `show route` and the VPN topology |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
