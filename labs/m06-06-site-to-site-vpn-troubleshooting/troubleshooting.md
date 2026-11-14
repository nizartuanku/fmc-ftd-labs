# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| Phase 1 fails right away | Pre-shared key mismatch | Compare the keys on both peers and look for the key error in the filtered debug |
| The console floods during a debug | The debug was not filtered | Use `debug crypto condition peer <PEER_IP>` first, and `undebug all` to stop |
| Status looks fine but you do not trust it | The management center cannot reach the device, so its views may be stale | Confirm management connectivity first |
| The tunnel is up but large transfers hang | MTU problem | Reduce MTU and retest with a large transfer |
| Nothing in the events | The configuration was not deployed to both devices | Deploy again and confirm the deployment status |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
