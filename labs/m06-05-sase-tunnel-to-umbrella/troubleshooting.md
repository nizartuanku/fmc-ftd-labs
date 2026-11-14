# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| Umbrella rejects the connection settings | A key, secret, token or Organization ID is wrong or mismatched | Re-enter each value from the Umbrella console and save again |
| You can create the topology but not deploy the tunnel | Export-controlled features are not enabled in the smart license | Enable them in the license account |
| The tunnel stays down | The Umbrella data center is not reachable from the threat defense | Check addressing, routing and outbound access to Umbrella |
| The VTI is up but traffic does not use it | No route sends the intended traffic into the tunnel | Check `show route` and `packet-tracer` |
| Deployment fails early | The SIG Essentials subscription is missing | Confirm the Umbrella subscription |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
