# Verification checklist

Work through this after the test steps. Do not assume it works: confirm each item.

- [ ] The internal CA is trusted by test clients.
- [ ] Do Not Decrypt exceptions sit above broad decrypt rules.
- [ ] Decrypt - Resign is used only for outbound traffic; Decrypt - Known Key only for servers you own.
- [ ] Connection events show the expected decryption result for each test site.
- [ ] On devices with TLS hardware acceleration, `show snort tls-offload` shows no rising fatal counters.
