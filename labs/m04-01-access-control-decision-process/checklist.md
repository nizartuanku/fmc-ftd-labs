# Verification checklist

Work through this after the test steps. Do not assume it works: confirm each item.

- [ ] Every Allow rule that carries user or internet traffic has a file policy and an intrusion policy attached (or a documented reason why not).
- [ ] Trust is used only for traffic you deliberately exempt from inspection.
- [ ] The default action is set intentionally, not left as an afterthought.
- [ ] `packet-tracer ... detailed` shows the expected access rule matching.
- [ ] Connection events show the intended rule; file/malware and intrusion events appear when the test file is downloaded.
