# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| The group never appears in IGMP | The receiver has not joined, or IGMP is not enabled on that interface | Check the receiver and the interface settings |
| No multicast route is created | PIM is not enabled toward the source | Check PIM on the source-facing interface |
| The stream is blocked | The access control policy does not allow the traffic | Add an allow rule for the group |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
