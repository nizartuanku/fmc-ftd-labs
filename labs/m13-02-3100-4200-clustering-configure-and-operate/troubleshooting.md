# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| A node fails to join | Hardware or version mismatch, CCL MTU too small on the switch, or a pending deployment | Use the predefined cluster outputs (`show cluster info`, `show cluster info health`, a CCL-sized ping) and see the design review lab |
| The cluster forms but data interfaces are missing | Data interfaces were configured before the cluster existed | Configure data interfaces after the cluster has formed |
| Management access is lost after failover | The main cluster IP was not what you used to manage | Manage through the main cluster IP |
| Interface errors in the wizard | Spanned EtherChannel and Individual interfaces are mixed | Use one type only |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
