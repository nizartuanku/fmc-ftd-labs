# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| The client connects but reaches nothing | No access control rule allows the VPN pool | Add the rule for the pool and deploy |
| Requests arrive but replies never reach the client | The dynamic PAT rule translates replies to the pool | Add the identity NAT exemption |
| The client cannot connect at all | Wrong access interface, certificate or missing Secure Client image | Check the access interface, the gateway certificate and the uploaded image |
| Authentication fails | The realm or RADIUS server is unreachable or credentials are wrong | Test the authentication server from the device |
| Internal names do not resolve | The group policy has no DNS settings | Set DNS in the group policy |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
