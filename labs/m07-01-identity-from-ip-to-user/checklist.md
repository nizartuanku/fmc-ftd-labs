# Verification checklist

Work through this after the test steps. Do not assume it works: confirm each item.

- [ ] The realm test succeeds and the user and group download completes.
- [ ] The identity policy is associated with the access control policy and deployed.
- [ ] Connection events show user names, not only IP addresses.
- [ ] A non-domain device is offered the captive portal (the fallback works).
- [ ] `show conn` on the threat defense shows the expected flows for the test hosts.
