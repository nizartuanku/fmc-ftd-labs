# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| No event for a test string | The protocol or port is not selected, or the threshold is higher than the number of matches | Select the protocol and port and check the threshold |
| The pattern is rejected | PCRE syntax was used instead of the simple syntax | Rewrite it with the documented characters and classes |
| FTP uploads are not inspected | The FTP data protocol, detector, port or file policy is missing | Meet each documented FTP requirement |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
