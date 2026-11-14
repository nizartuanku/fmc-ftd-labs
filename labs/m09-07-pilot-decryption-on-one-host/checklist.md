# Verification checklist

Work through this after the test steps. Do not assume it works: confirm each item.

- [ ] The internal CA is trusted on pilot clients.
- [ ] Exclusions are present as Do Not Decrypt rules above the decrypt rule.
- [ ] The decrypt rule is limited to the pilot host or subnet.
- [ ] The decryption policy is selected in the access control policy and deployed.
- [ ] Connection events show decryption only for pilot traffic.
- [ ] Trusted sites that stop loading are checked for certificate trust errors.
