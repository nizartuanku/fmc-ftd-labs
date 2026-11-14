# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| The connection test fails | ERS or Open API not enabled, CSRF check still on, or the ERS Operator user is wrong | Re-check the four ISE settings from Part 1 and the user's group |
| Certificate or trust errors during the connection | The internal CA is not enabled or the certificates are not trusted | Confirm the internal CA is enabled and review the quick configuration results |
| No SGTs in the rule editor | The integration is not connected or the topic is not subscribed | Check the identity source status and that Session Directory is subscribed |
| User names do not match the realm | Domain names differ between ISE and the management center realm | Align the domain names and re-download the realm |
| A destination SGT rule never matches | The SXP topic is not enabled, or SXP is not set up on ISE | Enable the SXP topic and SXP on ISE; remember SXP is not supported by ISE-PIC |
| Events show the user but not the SGT | The session has no SGT assigned in ISE | Check the authorization result for the client on ISE |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
