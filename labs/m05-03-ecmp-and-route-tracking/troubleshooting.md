# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| Only one default route is used | The metrics are different, so the routes are not equal | Give both routes the same metric |
| A dead path stays in the routing table | Route tracking is not enabled on the route or the target is the wrong address | Enable tracking toward a target beyond the next hop |
| The interface cannot join the zone | It is an unsupported type or already in another zone | Use a routed interface that is in no other zone |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
