# Verification checklist

Work through this after the test steps. Do not assume it works: confirm each item.

- [ ] Basic reachability first: `ping system` from the device CLI and `show network`.
- [ ] The management center shows the device healthy and connected, and the latest policy deployed successfully.
- [ ] `show nat detail`: translate hits increase on the intended rule, not on a broader rule above it.
- [ ] `packet-tracer ... detailed`: the NAT phase names the intended rule and the final result is allow.
- [ ] `show route`: routes to the inside server and back to the client are still valid.
- [ ] `show conn address <SERVER_IP>`: active connections with bytes in both directions.
