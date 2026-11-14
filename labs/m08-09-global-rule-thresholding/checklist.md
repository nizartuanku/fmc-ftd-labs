# Verification checklist

Work through this after the test steps. Do not assume it works: confirm each item.

- [ ] The global threshold is enabled, not disabled.
- [ ] Values were chosen from measured event volume, not guessed.
- [ ] Duplicate events for the same rule and destination dropped after deployment.
- [ ] Different rules and new targets still generate events.
- [ ] Drop rules still block traffic beyond the logging limit.
