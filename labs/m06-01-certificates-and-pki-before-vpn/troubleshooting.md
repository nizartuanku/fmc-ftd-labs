# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| The CA certificate will not paste or is rejected | The file is binary DER, not Base64 PEM text | Convert to Base64 PEM and check it starts with the BEGIN CERTIFICATE line |
| The identity certificate is rejected | The CA certificate is not installed on the device, or a different CA signed it | Install the correct CA first with Manual enrollment and CA Only, then import the identity certificate |
| The workflow asks for a certificate signing request when you only wanted the CA | CA Only is not checked | Edit the enrollment object and check CA Only |
| A VPN peer rejects the device certificate | The peer does not trust the CA that signed it | Make sure both sides trust the same CA, or the peer's CA chain is installed |
| Automatic enrollment never completes | The device cannot reach the CA | Check addressing and routing toward the CA |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
