# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| The client cannot connect, and no packet reaches the NAT rule | DNS returned only an A record | Enable DNS reply translation on the rule |
| A broader rule matches first | Rule order or interface scope is too wide | Order the NAT64 rule earlier and use specific interfaces |
| Replies never return | Upstream routes for the mapped addresses point elsewhere | Route the mapped addresses back to the firewall |
| The server is unreachable from the IPv6 side | No IPv6 prefix maps the IPv4 server | Add the mapping object and rule |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
