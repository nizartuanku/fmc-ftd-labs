# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| The non-compliant device still connects | The DAP is not associated with the RA VPN policy, or it was not deployed | Associate it in the RA VPN policy and deploy |
| Every device is rejected | The posture package is missing, so endpoint attributes are not reported | Upload the Secure Firewall Posture package (4.6 or later) |
| A compliant device is rejected | The endpoint criterion does not match the actual process name or state | Check the criterion against the real value on the client |
| Changes during a session do not apply | DAP is evaluated at connect time, not continuously | Reconnect to be evaluated again |
| Sessions are not visible in monitoring | Looking at the wrong view or the device is not reporting | Use active sessions and user activity, and check the device connection |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
