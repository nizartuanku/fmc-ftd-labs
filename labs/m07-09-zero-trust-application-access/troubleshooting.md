# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| The browser shows a certificate error for the application | The certificate does not match the application FQDN | Use a wildcard or SAN certificate that covers the FQDN |
| The FQDN does not resolve to the firewall | The DNS record is missing or points elsewhere | Resolve `<APP_FQDN>` from the client and confirm it returns the threat defense interface address |
| The login redirect to the identity provider fails | SAML settings or metadata do not match the identity provider | Re-check the application group's SAML settings against the provider |
| Nothing happens after deploy | The device does not run Snort 3, or the licence requirement is not met | Confirm Snort 3 and the export-controlled licence on the device |
| The application port is unreachable | The device HTTP server is on port 443 or the port pool is wrong | Move the device HTTP server off 443 and check the port pool |
| `show zero-trust` is empty after a test | The request never reached the application FQDN on the firewall | Check DNS, the zone and the counters in `show counters protocol zero_trust` |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
