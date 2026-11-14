# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| A container instance will not deploy on a module | The module previously ran a native instance and was not reinitialized | Reinitialize the security module first |
| A unit drops out of the cluster | CCL MTU or switch path problem, or a failed monitored interface | Check the CCL MTU on every hop and `show cluster info health` |
| The cluster will not form on a 9300 | Not all 3 modules are in the cluster | Include all modules (or a container instance on each) |
| Interface assignment is refused | A shared-type interface was used | Use dedicated interfaces |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
