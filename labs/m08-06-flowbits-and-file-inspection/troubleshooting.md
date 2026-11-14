# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| Rule B never fires | The flag names differ or Rule A never matched in the same flow | Compare the names and test Rule A alone |
| Rule B fires on everything | The isset check was left out | Add flowbits isset to Rule B |
| Archive inspection does nothing | The file policy has no file rules | Add at least one file rule |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
