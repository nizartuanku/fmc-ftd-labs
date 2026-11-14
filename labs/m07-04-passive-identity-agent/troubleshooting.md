# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| The agent never shows as connected | Wrong management center address or token, or the agent host cannot reach the management center | Re-enter `<FMC_ADDRESS>` and the token, and test network reachability from the agent host |
| Connected, but no user names in the events | The logon happened before the agent was connected, or the client does not pass through the threat defense | Log off and on again, and confirm the client traffic crosses the threat defense |
| A user shows as unknown | The user is not in the downloaded realm | Check the realm download and the Base DN and Group DN |
| Rules by user or group do not match | No identity policy with a passive rule is associated with the access control policy, or it is not deployed | Associate an identity policy with a passive rule for your zone and deploy |
| The secondary does not take over | The secondary agent is not configured or not connected | Confirm the second agent is connected to the management center before stopping the primary |
| A user still appears after logging off | The agent does not track logoffs | Expect this, and use a fresh logon to test |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
