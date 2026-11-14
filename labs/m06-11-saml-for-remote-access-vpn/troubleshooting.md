# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| The browser goes to a dead end after the IdP login | The base URL does not match what users reach | Correct the base URL on both sides |
| Valid logins are rejected | The clocks differ and the assertion looks expired or not yet valid | Fix NTP on the threat defense and compare with the IdP |
| The assertion signature fails validation | The IdP signing certificate in the SSO object is old or wrong | Re-import the current IdP certificate |
| Login works at the IdP but the VPN does not start | The profile still uses another authentication method | Select SAML and the right SSO object on the profile and deploy |
| The IdP shows an app error | Entity ID or reply URL mismatch | Compare the IdP application settings with the SSO object |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
