# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| An interface cannot be assigned to the virtual router | It is an EtherChannel member, redundant member or BVI member | Use a supported interface type |
| The route table looks empty | You ran `show route` for the global router, or used a management-only command | Use `show route vrf <name>` |
| A routing protocol will not start in the virtual router | User-defined virtual routers support only BGP and OSPFv2 | Use a supported protocol or static routes |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
