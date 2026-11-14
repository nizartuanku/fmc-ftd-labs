# Verification checklist

Work through this after the test steps. Do not assume it works: confirm each item.

- [ ] The engine version was confirmed before writing the rule.
- [ ] Every custom rule has at least one strong content match.
- [ ] Byte operations handle variable offsets instead of a broad regular expression.
- [ ] PCRE appears only after the content match.
- [ ] Latency and performance statistics were checked after the rule went live.
