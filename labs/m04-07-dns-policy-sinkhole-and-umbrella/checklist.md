# Verification checklist

Work through this after the test steps. Do not assume it works: confirm each item.

- [ ] The DNS policy is linked to the access control policy and deployed.
- [ ] Test lookups of listed domains return the sinkhole address or a not-found response.
- [ ] Connection and Security Intelligence events show hits for the sinkhole address or DNS rule.
- [ ] Hosts connecting to the sinkhole address are investigated as likely compromised.
- [ ] IP-based Security Intelligence remains in place for malware that skips DNS.
