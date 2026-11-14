# Verification checklist

Work through this after the test steps. Do not assume it works: confirm each item.

- [ ] Normal routing (`show route`) still sends general traffic out the primary ISP.
- [ ] `packet-tracer` shows matched traffic leaving the PBR egress interface.
- [ ] The PBR ACL matches only the intended traffic (no return traffic or internal flows).
- [ ] Path monitoring is enabled on the egress interfaces used with metric-based ordering.
- [ ] uRPF is disabled where PBR is applied.
- [ ] Failure behavior was tested in the lab, not assumed.
