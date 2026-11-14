# Verification checklist

Work through this after the test steps. Do not assume it works: confirm each item.

- [ ] The management connection is up and events are arriving.
- [ ] Failing connections were identified in Unified Events with TLS fields.
- [ ] Pinned applications have Do Not Decrypt exceptions.
- [ ] No OVER_SUBSCRIBED flags appear for normal load.
- [ ] Fatal counters stay at or near zero.
