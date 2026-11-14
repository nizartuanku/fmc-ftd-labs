# Verification checklist

Work through this after the test steps. Do not assume it works: confirm each item.

- [ ] The device was standalone, on a static Management IP and not onboarded by zero-touch provisioning.
- [ ] The configuration to rebuild was recorded before the conversion.
- [ ] `show system detail` shows the multi-instance (container) deploy mode.
- [ ] Each instance has a unique management IP on the shared Management interface.
- [ ] Each data interface is assigned to only one instance, and data-sharing interfaces are used only where allowed.
- [ ] Each instance registered to the management center as its own device.
