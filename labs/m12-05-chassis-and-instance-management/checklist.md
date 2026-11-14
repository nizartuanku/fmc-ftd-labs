# Verification checklist

Work through this after the test steps. Do not assume it works: confirm each item.

- [ ] `show system detail` shows the multi-instance (container) deploy mode.
- [ ] The prompt shows the generic firepower-model name, not the old hostname.
- [ ] The chassis Management interface has a static IP and no data interface is used for chassis management.
- [ ] A Chassis Platform Settings policy is assigned to the chassis.
- [ ] Each instance has its own management IP, different from the chassis IP.
- [ ] Each instance is registered and healthy as a separate device in the management center.
