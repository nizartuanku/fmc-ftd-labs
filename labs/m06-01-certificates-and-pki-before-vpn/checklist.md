# Verification checklist

Work through this after the test steps. Do not assume it works: confirm each item.

- [ ] The CA certificate was provided in Base64 PEM format.
- [ ] The CA certificate is installed before the identity certificate.
- [ ] `show crypto ca certificates` shows the expected CA with status Available and valid dates.
- [ ] The identity certificate is signed by a CA the peer also trusts.
- [ ] CA and identity certificate expiry dates are tracked (calendar or monitoring).
- [ ] For automatic enrollment, the device can reach the CA (check addressing and routing; `show network` displays the management interface settings).
