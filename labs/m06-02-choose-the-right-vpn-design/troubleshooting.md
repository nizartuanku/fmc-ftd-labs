# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| The VPN option is greyed out or strong ciphers are missing | Export-controlled functionality is not enabled in the license | Check the smart license and its export-controlled setting |
| The tunnel is up but no traffic passes | Missing routes, access rules or protected network mismatch | Check routing and the protected networks on both peers |
| Traffic through a transparent firewall is not encrypted | Transparent mode does not terminate through traffic for VPN | Use routed mode for VPN termination |
| Remote access cannot be configured on a cluster | Remote access VPN is not supported on clusters | Terminate remote access on standalone or high-availability devices |
| Cluster VPN tunnels drop after a failover | VPN runs on the control node only | Expect tunnels to re-establish after a new control node is elected |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
