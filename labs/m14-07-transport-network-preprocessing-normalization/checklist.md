# Verification checklist

Work through this after the test steps. Do not assume it works: confirm each item.

- [ ] The inspection engine is Snort 2 for these settings.
- [ ] Checksum verification actions are deliberate (verify or drop).
- [ ] IP Defragmentation and Inline Normalization are enabled where required.
- [ ] Inline Mode is on and the device is deployed inline if you expect normalization or drops.
- [ ] Fragment Settings (Chain, Size and Timeout) are known and documented.
- [ ] `show asp drop` and intrusion events reflect expected fragment handling.
