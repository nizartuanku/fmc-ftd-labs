# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| User finishes the Microsoft login but is treated as **Unknown** | The SSO application's attributes do not match what the realm expects | Compare the attribute mapping in the SSO application with the realm settings, and re-check the identifier values in the realm |
| Groups do not appear in the realm | Wrong identifier values, or the trust is not established | Re-check the values collected from Entra ID, and confirm the certificate has not expired |
| Users silently dropped, no alarms, empty logs | Platform user or group limit exceeded, so identity sync fails silently | Look up the maximum users and groups for your platform in the guide before syncing a large tenant |
| Captive portal redirect does not happen | The Decrypt - Resign rule is missing or does not cover these users | The firewall must decrypt HTTPS to redirect the user to the portal. Add or fix the Decrypt - Resign rule |
| Everyone lands in Unknown / Failed Authentication | No explicit rules for special identities, so the default action applies | Add explicit rules for Unknown, Failed Authentication, Guest and No Authentication Required |
| It worked, then stopped | An expired certificate in the SSO trust | Check certificate validity on both sides |

## Habits that prevent most lockouts

- Monitor for realm or user mismatches. They are almost always the top cause.
- Define fallback rules for the special identities up front.
- Verify with a live test account under your active or passive conditions after every
  change, and check user downloads in the management center.

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
