# Verification checklist

Work through this after the test steps. Do not assume it works: confirm each item.

- [ ] The tunnel source is a routed interface or loopback, not a bridge group.
- [ ] The public IP option is set when the VPN interface is behind NAT or PAT.
- [ ] `show route` shows the remote subnets via the VTI (static or dynamic).
- [ ] `packet-tracer` confirms traffic enters the tunnel, not the default route.
- [ ] `show crypto ipsec sa` shows encrypt and decrypt counters increasing.
- [ ] The backup tunnel and metrics were tested by failing the primary path.
- [ ] MTU was checked with large transfers.
