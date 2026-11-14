# Verification checklist

Work through this after the test steps. Do not assume it works: confirm each item.

- [ ] The engine is Snort 2 for these settings.
- [ ] Portscan Detection is enabled with the intended sensitivity; stream preprocessing is enabled.
- [ ] GID 122 rules are enabled for the scan types in use.
- [ ] The portscan packet view shows the expected scanner IP, target and port range.
- [ ] Rate-based thresholds are based on a measured baseline; inline versus passive behavior is understood.
- [ ] Legitimate peak traffic is not dropped.
