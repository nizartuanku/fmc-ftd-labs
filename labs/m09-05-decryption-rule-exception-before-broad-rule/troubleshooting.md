# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| An application fails after decryption is enabled | It pins its certificate and rejects the re-signed one | Add a Do Not Decrypt rule for it above the decrypt rule |
| Browsers show certificate warnings | Clients do not trust the internal CA | Distribute the CA certificate to clients |
| The exception has no effect | It sits below the broad decrypt rule | Move it above |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
