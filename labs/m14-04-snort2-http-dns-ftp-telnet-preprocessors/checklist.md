# Verification checklist

Work through this after the test steps. Do not assume it works: confirm each item.

- [ ] The device inspection engine is Snort 2 for these settings.
- [ ] Custom NAP changes are committed, not left as unsaved changes.
- [ ] HTTP Inspect, DNS and FTP/Telnet are enabled only where needed.
- [ ] Inline Mode is enabled and the device is deployed inline if you expect normalization or drops.
- [ ] The NAP is assigned and deployed; intrusion events show the expected rule hits.
