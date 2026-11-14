# Verification checklist

Work through this after the test steps. Do not assume it works: confirm each item.

- [ ] SIG Essentials subscription and export-controlled licensing are in place.
- [ ] Umbrella connection settings are complete and accepted.
- [ ] The SASE tunnel status in the management center shows up.
- [ ] `show interface ip brief` shows the VTI up.
- [ ] `show crypto ipsec sa` shows encrypt and decrypt counters increasing.
- [ ] `show route` and `packet-tracer` confirm the intended traffic enters the tunnel.
