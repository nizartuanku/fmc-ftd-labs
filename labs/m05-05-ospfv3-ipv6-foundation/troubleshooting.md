# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| No OSPFv3 neighbor appears | IPv6 is not enabled, or the link-local address has a duplicate | Check `show ipv6 interface brief` and syslog 325002 |
| The interface has no global address | Enable IPv6 creates only the link-local address | Add a global address or use DHCPv6 prefix delegation |
| Management IPv6 looks fine but OSPFv3 is down | Management addressing commands do not configure data interfaces | Verify the data plane with the ipv6 show commands |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
