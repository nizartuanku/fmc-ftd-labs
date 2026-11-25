# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| No events in Splunk | Wrong certificate or password, or the port is blocked | Re-download the certificate and check connectivity |
| Inputs missing on the search head | Distributed deployment | Configure inputs on the heavy forwarder |
| AI Assistant answer looks old | Policy data syncs up to every 24 hours | Allow time for the next sync |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
