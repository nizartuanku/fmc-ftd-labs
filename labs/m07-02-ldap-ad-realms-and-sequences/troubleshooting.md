# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| Test fails with a name resolution error | The management center cannot resolve the directory host name | Check the host name and the DNS server the management center uses; try the IP address to isolate DNS |
| Test fails only after enabling LDAPS or STARTTLS | Missing or wrong CA certificate, a certificate name that does not match the host, or the wrong port | Confirm the CA chain, use the name that appears in the certificate, and check the port |
| Bind or authentication failure | Wrong service account name or password, or the account lacks read rights | Verify the account format and password and try a different known-good account |
| The download completes but groups are missing | The Group DN or Base DN is too narrow | Re-check both DNs with Fetch DNs and download again |
| User and group download fails or stops | The directory became unreachable during the download | Check the realm status and health messages, and see the guide's realm troubleshooting section |
| An LDAP realm cannot be added to a sequence | Realm sequences accept only Active Directory realms | Use AD realms in the sequence |
| Access rules do not match the expected users | The group was not downloaded or the rule uses a different realm | Confirm the group exists in the realm you selected and that the policy is deployed |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
