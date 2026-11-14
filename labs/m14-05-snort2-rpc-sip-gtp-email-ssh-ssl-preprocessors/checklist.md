# Verification checklist

Work through this after the test steps. Do not assume it works: confirm each item.

- [ ] The NAP targets the right networks and is deployed.
- [ ] Only the preprocessors your network needs are enabled.
- [ ] Preprocessor rules have the intended action in the intrusion policy.
- [ ] Snort Fail Open Busy and Down settings are a deliberate choice for each inline set.
- [ ] Encrypted traffic you must inspect is covered by a decryption policy, not by the SSH or SSL preprocessors.
