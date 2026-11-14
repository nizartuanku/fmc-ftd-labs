# Verification checklist

Work through this after the test steps. Do not assume it works: confirm each item.

- [ ] Chassis-level SNMP is configured on each Firepower 1000, not only in the Platform Settings policy.
- [ ] Community strings contain none of @, backslash, ? or spaces (v1/v2c), or SNMPv3 priv is used.
- [ ] ISA 3000 alarm status is visible in the management center.
- [ ] Syslog shows the physical alarm events.
- [ ] A test trigger produces a trap at the monitoring server.
