# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| Clients cannot reach the gateway | The profile is bound to the wrong interface | Bind it to the internet-facing interface in the outside zone |
| A user gets the wrong group policy | The authorization server or the profile decides differently than expected | Test both outcomes and check which one is in control |
| No address is assigned | The selected assignment source is empty or unreachable | Check the pool, DHCP server or AAA authorization attribute |
| One pool works, the other does not | Access rule or NAT exemption covers only one pool | Add both to rules and NAT |
| Split tunneling shows no effect | The client was not reconnected after deployment | Reconnect and compare the route table |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
