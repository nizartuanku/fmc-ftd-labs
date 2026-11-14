# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| No EIGRP neighbor appears | AS number mismatch, interface not in the process, or no reachability | Compare the AS number and the interface network on both sides |
| EIGRP cannot be configured on an interface | It is an EtherChannel member or belongs to a user-defined virtual router | Use a supported interface in the global virtual router |
| Routing loops after redistribution | No route tagging between EIGRP and OSPF | Configure route tagging |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
