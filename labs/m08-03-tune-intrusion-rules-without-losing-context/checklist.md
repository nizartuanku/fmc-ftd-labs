# Verification checklist

Work through this after the test steps. Do not assume it works: confirm each item.

- [ ] Engine version and IPS license were confirmed before tuning.
- [ ] The noisy rule was identified by its SID, not by guessing.
- [ ] The suppression is scoped to the scanner address only and the rule is still enabled.
- [ ] A test from a different host still generates an event.
- [ ] The reason for the tuning is recorded as a comment and in the change record.
- [ ] The policy was deployed and the change appears in the deployment history.
