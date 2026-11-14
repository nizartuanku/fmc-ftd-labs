# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| User-based access rules never match | The identity policy is not associated with the access control policy, or it was not deployed | Open the access control policy's advanced settings and confirm the association, then deploy |
| An FQDN object is rejected in an identity rule | FQDN network objects are supported only in access control, prefilter and manual NAT rules | Use an IP network object in the identity rule |
| Finance users appear as Unknown | No passive mapping and the rule does not fall back to active authentication | Confirm the passive source works and that the fallback option is enabled |
| Guest users are never prompted | The guest zone or network does not match Rule 2, or the rule order is wrong | Check the zone, network and order of the identity rules |
| Everyone is blocked after deployment | The Unknown block rule sits above the identity-based allow rules | Reorder the access rules so identified users are evaluated first |
| The finance group is missing in the rule editor | The realm did not download the group | Re-run the realm download and check the Group DN |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
