# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| Connection events show IP addresses but no users | No passive mapping and no active fallback for that host, or the identity policy is not associated with the access control policy | Confirm the identity policy is selected in the access control policy settings and deployed; check the rule's zone and realm |
| Realm test fails | Wrong host, port or credentials, or DNS cannot resolve the directory | Test the host name from the management center side; check the service account and the Base DN |
| The group is missing in the access rule editor | The user and group download did not complete, or the group is outside the Group DN | Re-run the download and check the Group DN and the realm health messages |
| The captive portal never appears for the non-domain VM | Fallback not enabled, rule does not match the zone, or the HTTPS traffic is not decrypted | Check rule order and zone; confirm the decryption policy has Decrypt - Resign for Unknown users and is associated |
| Browser certificate warnings on HTTPS sites | The lab VM does not trust the Decrypt - Resign CA | Install the lab CA certificate in the client trust store |
| A realm sequence is not accepted in a captive portal rule | Realm sequences are not supported in captive portal rules | Use a single realm in active-authentication rules |
| `show conn` shows nothing for the host | The traffic is not reaching the threat defense, or the client has a different IP than expected | Confirm the client address and path, then compare with the connection events |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
