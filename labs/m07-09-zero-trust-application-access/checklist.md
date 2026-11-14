# Verification checklist

Work through this after the test steps. Do not assume it works: confirm each item.

- [ ] `show running-config zero-trust` on the threat defense shows the deployed configuration.
- [ ] `show zero-trust` shows sessions and statistics after a test login.
- [ ] `show counters protocol zero_trust` shows counters increasing during tests.
- [ ] Connection events include the Zero Trust Application field, and the Zero Trust dashboard lists top applications and users.
- [ ] Unpublished internal hosts are not reachable from the client.
