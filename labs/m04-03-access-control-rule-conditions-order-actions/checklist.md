# Verification checklist

Work through this after the test steps. Do not assume it works: confirm each item.

- [ ] Specific rules sit above general rules.
- [ ] Application conditions are used instead of port-only conditions where possible.
- [ ] Rules with user conditions have an identity policy associated with the access control policy.
- [ ] No rule-conflict or shadowing warnings remain.
- [ ] Hit counts increase on the intended rules; a rule stuck at zero is misplaced or misconfigured.
- [ ] `packet-tracer ... detailed` names the expected rule for a test flow.
