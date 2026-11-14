# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| A known-bad file downloads through an Allow rule | No file or intrusion policy is attached to the rule | Attach inspection policies to every Allow rule that carries user traffic |
| Traffic is blocked even though the rule allows it | The file or intrusion policy blocked it after the Allow | Check the file/malware and intrusion events |
| The wrong rule matches | A rule above it matches first | Review the rule order and use packet-tracer |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
