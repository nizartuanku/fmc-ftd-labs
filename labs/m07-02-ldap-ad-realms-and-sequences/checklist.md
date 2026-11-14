# Verification checklist

Work through this after the test steps. Do not assume it works: confirm each item.

- [ ] The directory Test succeeds (with LDAPS after adding the CA certificate).
- [ ] The user and group download completes and the expected groups appear.
- [ ] The realm sequence contains only Active Directory realms, in the intended order.
- [ ] Access rules that use the downloaded groups match traffic (connection events show the user).
- [ ] No realm or user mismatches remain (see the guide's troubleshooting section for realms and user downloads).
