# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| MFA push fails before the user can approve | The RADIUS timeout is still the 10-second default | Raise it to 60 seconds or more |
| Users without a certificate still get in | The profile is not set to require the certificate | Use certificate and AAA and test from a machine without a certificate |
| A user gets the wrong or default group policy | RADIUS returns a name that does not match the deployed policy | Create the group policy with the exact name and deploy |
| RADIUS timeouts for everyone | Wrong shared secret, address or routing to the server | Check secret, address and reachability from the device |
| No accounting records | Accounting is not enabled on the profile or server | Enable accounting and check the RADIUS server logs |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
