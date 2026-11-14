# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| No traps arrive | The SNMP manager is missing from the chassis-level settings, or the credentials or level do not match | Check the manager entry, SNMPv3 user and security level |
| Trap parsing fails | The community string contains @, backslash, ? or a space | Use a simple string or SNMPv3 |
| The dashboard is green during overheating | Only traffic and security logs are monitored, not hardware | Add chassis-level SNMP and the physical alarms |
| Alarms never fire in the lab | The thresholds or input contacts were not enabled | Enable the alarm types and redeploy |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
