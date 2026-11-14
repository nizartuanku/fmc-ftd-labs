# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| The tunnel is up but nothing is encrypted | No route points the remote subnet at the VTI | Add a route over the VTI; confirm with `show route` and `packet-tracer` |
| Traffic leaves the WAN unencrypted | The default route wins over a missing specific route | Add the specific route toward the VTI |
| Negotiation fails behind NAT | The peer sees a private address | Enable the public IP option and enter the post-NAT address |
| The VTI cannot be created on the chosen interface | The source is a bridge group member or transparent mode | Use a routed interface or a loopback |
| Apps connect but large transfers hang | MTU not adjusted for IPsec overhead | Lower the MTU and retest with a large transfer |
| The backup VTI never takes over | Backup route metric is not worse than the primary, or the primary stays reachable | Check metrics and that the primary path really fails |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
