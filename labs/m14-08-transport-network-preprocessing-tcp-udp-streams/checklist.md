# Verification checklist

Work through this after the test steps. Do not assume it works: confirm each item.

- [ ] The inspection engine is confirmed (these are Snort 2 settings).
- [ ] TCP and UDP stream preprocessing are enabled in the NAP in use.
- [ ] Reassembly ports and services cover the protected applications.
- [ ] The cluster is healthy (`show cluster info`) and TCP sequence randomization is left enabled.
- [ ] The TCP MSS value is chosen deliberately for IPsec or non-IPsec use.
- [ ] Test traffic was not blocked or fastpathed before inspection.
