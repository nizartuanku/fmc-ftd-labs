# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| CPU and latency rise after the rule | The rule relies on PCRE alone, so every matching packet is checked expensively | Add a strong content match before the PCRE |
| A variant payload is missed | The content or PCRE is too literal, or the offset changes | Use byte operations or a case-insensitive pattern |
| A replace rule corrupts traffic | The replacement is not the same length as the matched content | Use a replacement of equal length |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
