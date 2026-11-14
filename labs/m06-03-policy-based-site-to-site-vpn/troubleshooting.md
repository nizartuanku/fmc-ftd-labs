# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| The tunnel never comes up | No common IKE or IPsec proposal, or a pre-shared key mismatch | Compare both peers' IKE and IPsec parameters and the key; read the VPN troubleshooting logs |
| The policy will not deploy | The device is not registered or not reachable from the management center | Check device registration and the management channel |
| The tunnel is up but traffic is not encrypted | The protected networks do not match what is being sent | Check that both peers list the same subnets, mirrored |
| Only some subnets work | A subnet is missing from one side's protected networks | Add it to both peers and deploy |
| VPN breaks after a cluster failover | Only the control node runs VPN | Expect re-establishment after the new control node is elected |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
