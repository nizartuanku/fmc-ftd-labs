# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| An instance cannot be reached | It reuses the chassis management IP or an address already in use | Give every instance a unique address on the Management network |
| The chassis loses management after a change | Management was moved to DHCP or to a data interface | Use the dedicated Management interface with a static IP |
| Chassis settings do not apply | The Chassis Platform Settings policy is not assigned to the chassis | Assign the policy and deploy again |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
