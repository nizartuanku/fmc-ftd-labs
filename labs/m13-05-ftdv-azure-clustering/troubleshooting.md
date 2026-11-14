# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| Registration with the management center fails | A shared requirement was missed: mixed tier, missing Day 0 setting, VPN on a data node or an unlicensed management center | Re-check the requirement table in the background section |
| Data units leave and rejoin after licensing | The cluster was added while the management center was in evaluation mode | License first |
| The function upload fails | Wrong or missing user-scope FTPS credentials | Recreate the credentials in Deployment Center |
| Poor performance with a small cluster | The CCL IP range is much larger than needed | Use the smallest range that covers your nodes |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
