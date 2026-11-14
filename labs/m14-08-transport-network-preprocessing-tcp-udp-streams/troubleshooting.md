# Troubleshooting

| Symptom | Likely cause | What to check |
|---|---|---|
| Segmented attacks are not detected | Stream reassembly is not enabled for the relevant ports or services | Enable reassembly for those ports or services |
| Sessions fail to establish in a cluster | TCP sequence randomization was disabled | Leave it enabled in a cluster |
| Large transfers fail through an IPsec tunnel | MSS leaves too little room for VPN overhead | Choose the MSS for IPsec use |
| No intrusion events for test traffic | Traffic was blocked earlier or fastpathed by a prefilter rule | Check access control, prefilter and packet-tracer |

---
*Always confirm behavior against the guide for your exact FMC/FTD version.*
