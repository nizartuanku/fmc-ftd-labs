# Verification checklist

Work through this after the test steps. Do not assume it works: confirm each item.

- [ ] `show route`: two default routes with identical metrics while both paths are healthy.
- [ ] `show sla monitor operational-state`: probes report success for each path.
- [ ] After a simulated upstream failure, the failed path's route disappears from `show route`.
- [ ] `packet-tracer ... detailed` for two different flows shows the expected egress interfaces.
- [ ] No more than 8 interfaces in the zone; each interface in only one zone.
