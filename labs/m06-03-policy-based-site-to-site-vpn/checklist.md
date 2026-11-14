# Verification checklist

Work through this after the test steps. Do not assume it works: confirm each item.

- [ ] Topology and protected networks are documented for both sites.
- [ ] Both devices are registered and the VPN policy is deployed to both.
- [ ] IKE and IPsec proposals have at least one exact match on both peers.
- [ ] Tunnel status is up in the management center and `show crypto ipsec sa` shows encrypt and decrypt counters increasing.
- [ ] In a cluster, VPN is configured only for the control node, and the team knows tunnels drop on control-node failover.
