# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| The limit has no effect | The traffic is fastpathed by a prefilter rule, or the rule is on a VTI or VPN path | Use a routed interface and make sure access control allows or trusts the traffic |
| A broader rule limits the wrong traffic | First match wins and the broader rule is above | Put specific rules first |
| No QoS information in events | Connection logging is not enabled at the end of connection | Enable Log at End of Connection on the access rule |
| Total bandwidth is higher than the configured limit | The limit is per interface, not shared across interfaces | Account for the per-interface limit |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
