# Verification checklist

Work through this after the test steps. Do not assume it works: confirm each item.

- [ ] The device is in routed mode.
- [ ] `show ospf neighbor`: neighbor state FULL on the expected interface.
- [ ] `show route`: O, O IA or O E1/E2 routes present as designed.
- [ ] Summaries and filters behave as intended (expected prefixes present, filtered prefixes absent).
- [ ] The configuration was deployed from the management center (no pending changes).
