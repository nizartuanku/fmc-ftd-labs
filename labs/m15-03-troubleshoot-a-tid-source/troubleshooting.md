# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| A source shows an error or stops updating | Certificate or hostname verification fails, or the feed format is wrong | Check the source's SSL Settings and content requirements |
| Observables are not enforced on a device | The management connection is down | Check `sftunnel-status-brief` and the element status |
| Two incidents for one indicator | The indicator exists in two published copies | Pause publishing on all but one copy |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
