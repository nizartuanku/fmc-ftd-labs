# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| Nothing is decrypted | The policy is not selected in the access control policy, or was not deployed | Select it in Advanced settings and deploy |
| A sensitive site was decrypted | The exclusion is missing or below the decrypt rule | Check the generated Do Not Decrypt rules and their order |
| A trusted site stops loading | Certificate trust errors on the re-signed certificate | Check trust for the issuing CAs and add an exception if needed |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
