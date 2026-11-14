# FMC & FTD labs

Hands-on lab outlines for the **Cisco Secure Firewall (FMC & FTD)** video series on the
[Hexward Labs YouTube channel](https://www.youtube.com/@nizartuanku).

Each lab is a self-contained folder: goal, prerequisites, numbered steps, a verification
checklist and troubleshooting notes. All environment-specific values are placeholders
(for example `<TENANT_ID>`), so nothing here contains real tenant data or secrets.

> **Use a lab FMC/FTD or a virtual lab, never production.**

## Labs

| Lab | Video | Topic |
|---|---|---|
| [m06-01-certificates-and-pki-before-vpn](labs/m06-01-certificates-and-pki-before-vpn/) | [Certificates and PKI Before VPN Configuration](https://youtu.be/FJkeLd4PbO4) | Install a CA certificate first, then an identity certificate, and verify both on the device |
| [m06-02-choose-the-right-vpn-design](labs/m06-02-choose-the-right-vpn-design/) | [FTD VPNs: Site-to-Site or Remote Access?](https://youtu.be/sgVSWo46yb8) | Check licensing and routed mode, build a simple site-to-site tunnel and write down where remote access can terminate |
| [m06-03-policy-based-site-to-site-vpn](labs/m06-03-policy-based-site-to-site-vpn/) | [Policy-Based Site-to-Site VPN](https://youtu.be/uzTQBjUM9gc) | Build a policy-based tunnel, break it with a mismatched IKE proposal and find the mismatch in the logs |
| [m06-04-route-based-vpn-with-vti](labs/m06-04-route-based-vpn-with-vti/) | [Route-Based VPN with VTI](https://youtu.be/a4xt_ddFoQE) | Build a static VTI tunnel, prove that routing decides what is encrypted, add a backup VTI and check MTU |
| [m06-05-sase-tunnel-to-umbrella](labs/m06-05-sase-tunnel-to-umbrella/) | [SASE Integration Through Site-to-Site VPN](https://youtu.be/fWwqmqK0kx4) | Register Umbrella with the management center, build the SASE tunnel and verify the VTI and security association |
| [m06-06-site-to-site-vpn-troubleshooting](labs/m06-06-site-to-site-vpn-troubleshooting/) | [Verifying and Troubleshooting Site-to-Site VPN](https://youtu.be/q6XQ12ealyk) | Break a tunnel with a wrong pre-shared key, then follow dashboard, events and filtered debugs to the cause |
| [m06-07-remote-access-vpn-basic-configuration](labs/m06-07-remote-access-vpn-basic-configuration/) | [Remote Access VPN: Preparation and Basic Configuration](https://youtu.be/l4d26d7S59M) | Build a basic RA VPN policy and add the access rule and NAT exemption that turn a login into reachability |
| [m06-08-remote-access-profiles-and-group-policies](labs/m06-08-remote-access-profiles-and-group-policies/) | [Remote Access VPN: Profiles, Interfaces, and Advanced Settings](https://youtu.be/hz7m2y2Tdps) | Bind profiles to the access interface, compare address assignment options and see profile versus group policy |
| [m06-09-split-tunneling-management-tunnel-client-modules](labs/m06-09-split-tunneling-management-tunnel-client-modules/) | [Split Tunneling, Management Tunnels, and Client Modules](https://youtu.be/0qHTNDs6CNY) | Compare full and split tunneling, try dynamic split by domain and build a certificate-based management tunnel |
| [m06-10-remote-access-authentication-aaa-certs-mfa](labs/m06-10-remote-access-authentication-aaa-certs-mfa/) | [Remote Access Authentication: AAA, Certificates, and MFA](https://youtu.be/-tkC_x-cQp4) | Move from password-only to certificate plus AAA, add secondary authentication and fix the MFA timeout |
| [m06-11-saml-for-remote-access-vpn](labs/m06-11-saml-for-remote-access-vpn/) | [SAML for Remote Access VPN](https://youtu.be/-xZeJ1EyCJw) | Create the IdP application and the SSO server object, log in with Secure Client and break the base URL on purpose |
| [m06-12-dynamic-access-policies-and-vpn-monitoring](labs/m06-12-dynamic-access-policies-and-vpn-monitoring/) | [Dynamic Access Policies and VPN Session Monitoring](https://youtu.be/H4LoKcCsGqs) | Build a DAP with a posture requirement, prove it only works once associated and monitor the sessions |
| [m07-01-identity-from-ip-to-user](labs/m07-01-identity-from-ip-to-user/) | [Cisco FMC Identity Policy Tutorial: User-Based Access Control with Cisco FTD](https://youtu.be/KFklKLNshSg) | Turn IP addresses into users with a realm, an identity policy, decryption and a group-based access rule |
| [m07-02-ldap-ad-realms-and-sequences](labs/m07-02-ldap-ad-realms-and-sequences/) | [LDAP/AD Realms, Realm Sequences, and Troubleshooting](https://youtu.be/2T4nDKTXR5U) | Build a realm, encrypt the directory connection, create a realm sequence and learn the failure messages |
| [m07-03-azure-ad-saml-realm](labs/m07-03-azure-ad-saml-realm/) | [Microsoft Azure AD Realms in the SAML Context](https://youtu.be/3fGXzAuIIyk) | Map Microsoft Entra ID identities to firewall access control with a Microsoft Azure AD (SAML) realm |
| [m07-04-passive-identity-agent](labs/m07-04-passive-identity-agent/) | [Passive Identity Agent: Recognizing Users Without a Login Portal](https://youtu.be/ioKDqCbZGgE) | Install a passive identity agent, map logons to IP addresses and test a secondary agent |
| [m07-05-cisco-ise-identity-source](labs/m07-05-cisco-ise-identity-source/) | [Integrating Cisco ISE or ISE-PIC](https://youtu.be/jvftEmY0c2o) | Integrate a lab Cisco ISE node, use SGTs as source and destination conditions, and learn when SXP matters |
| [m07-08-building-identity-policies](labs/m07-08-building-identity-policies/) | [Building and Verifying Identity Policies](https://youtu.be/EsXA-S-EAkk) | Build an identity policy with passive and active rules, handle special identities and prove the association matters |
| [m07-09-zero-trust-application-access](labs/m07-09-zero-trust-application-access/) | [Cisco FMC Zero Trust Application Access (ZTNA): Policies, App Groups & Monitoring](https://youtu.be/W7tDtA2p-Lo) | Publish one web application behind the firewall with a Zero Trust Application policy and a SAML identity provider |
| [m13-01-3100-4200-clustering-design-review](labs/m13-01-3100-4200-clustering-design-review/) | [Cisco FMC & FTD: Secure Firewall 3100/4200 Clustering: Design and Prerequisites](https://youtu.be/1cW2ajxX1ZQ) | Check hardware, software, time, the cluster control link and the data interface type before you touch the Add Cluster wizard |
| [m13-02-3100-4200-clustering-configure-and-operate](labs/m13-02-3100-4200-clustering-configure-and-operate/) | [Cisco FMC & FTD: 3100/4200 Clustering: Configuration and Operations](https://youtu.be/SvBu7cukoSo) | Build a two-node cluster in the management center, watch its health and prove control-node failover |
| [m13-03-ftdv-private-cloud-clustering](labs/m13-03-ftdv-private-cloud-clustering/) | [Cisco Secure Firewall: FTD Virtual Clustering in Private Clouds](https://youtu.be/PAU_8SGoBR4) | Deploy two virtual nodes with the Day 0 cluster setting, form the cluster and prove control-node failover |
| [m13-04-ftdv-aws-clustering](labs/m13-04-ftdv-aws-clustering/) | [Cisco Secure Firewall: FTD Virtual Clustering on AWS](https://youtu.be/5rM27fVZSSM) | Check the tier, licensing and template inputs, then verify the cluster status and the GWLB failover setting |
| [m13-05-ftdv-azure-clustering](labs/m13-05-ftdv-azure-clustering/) | [Cisco Secure Firewall: FTD Virtual Clustering on Azure](https://youtu.be/GdeFtGYq9sM) | Check the shared requirements, size the CCL range, deploy the template and upload the cluster function |
| [m13-06-ftdv-google-cloud-clustering](labs/m13-06-ftdv-google-cloud-clustering/) | [Cisco Secure Firewall: FTD Virtual Clustering on Google Cloud](https://youtu.be/-lbVosdSnwY) | Prepare the Day 0 script and MTUs, list the Google Cloud objects to build and add the control node |
| [m13-07-4100-9300-clustering-design-and-bootstrap](labs/m13-07-4100-9300-clustering-design-and-bootstrap/) | [Cisco FMC & FTD: Firepower 4100/9300 Clustering: Design and Configuration](https://youtu.be/IDfgMjM4Oic) | Check hardware mixing, size the CCL on Port-channel 48, reinitialize modules and bootstrap the cluster from the chassis |
| [m13-08-4100-9300-clustering-troubleshooting](labs/m13-08-4100-9300-clustering-troubleshooting/) | [Cisco FMC & FTD: 4100/9300 Clustering: Management and Troubleshooting](https://youtu.be/uRdF1Dsswf4) | Read the cluster status views, run the predefined cluster CLI and prove a CCL MTU mismatch with a large ping |
| [m14-01-flexconfig-safe-workflow](labs/m14-01-flexconfig-safe-workflow/) | [Cisco FMC & FTD: FlexConfig: When to Use It and How to Manage It](https://youtu.be/QDGbceWxIvE) | Pick a feature the GUI does not manage, build text and FlexConfig objects, preview, deploy, verify and plan the removal |
| [m14-02-flexconfig-examples-and-migration](labs/m14-02-flexconfig-examples-and-migration/) | [Cisco FMC & FTD: FlexConfig: Examples, Migration, and Configuration Review](https://youtu.be/pZ0yHrzGAfs) | Match an example to your hardware, preview and deploy it, then review FlexConfig objects for features that are now managed |
| [m14-03-advanced-access-control-and-nap](labs/m14-03-advanced-access-control-and-nap/) | [Cisco FMC & FTD: Advanced Access Control and Network Analysis Policies](https://youtu.be/JRBFEt5FacE) | Set the default network analysis policy and the intrusion policy used before an access rule is determined, with a custom NAP for one subnet |
| [m14-04-snort2-http-dns-ftp-telnet-preprocessors](labs/m14-04-snort2-http-dns-ftp-telnet-preprocessors/) | [Cisco FMC & FTD: Snort 2: HTTP, DNS, and FTP/Telnet Preprocessors](https://youtu.be/Ini0h4ADak0) | Enable HTTP Inspect in a custom NAP, add a server-level configuration and see why rules must match the normalized form |
| [m14-05-snort2-rpc-sip-gtp-email-ssh-ssl-preprocessors](labs/m14-05-snort2-rpc-sip-gtp-email-ssh-ssl-preprocessors/) | [Cisco FMC & FTD: Snort 2: RPC, SIP, GTP, Email, SSH, and SSL Preprocessors](https://youtu.be/eKbkzyKgKdg) | Enable the SIP preprocessor, set its rules to alert or drop and record the inline set Snort Fail Open options |
| [m14-06-snort2-scada-preprocessors-for-ot](labs/m14-06-snort2-scada-preprocessors-for-ot/) | [Cisco FMC & FTD: Snort 2 for OT: Modbus, DNP3, CIP, and S7](https://youtu.be/ogFACtAY8lE) | Inventory industrial protocols and ports, set the Modbus preprocessor ports to match, and confirm inspection with the N flag in show conn |
| [m14-07-transport-network-preprocessing-normalization](labs/m14-07-transport-network-preprocessing-normalization/) | [Cisco FMC & FTD: Transport/Network Preprocessing: Normalization and Defragmentation](https://youtu.be/dUiIW6z1n8M) | Review checksum verification, IP defragmentation and inline normalization in a Snort 2 NAP and record the separate threat defense fragment settings |
| [m14-08-transport-network-preprocessing-tcp-udp-streams](labs/m14-08-transport-network-preprocessing-tcp-udp-streams/) | [Cisco FMC & FTD: Transport/Network Preprocessing: TCP and UDP Streams](https://youtu.be/PjsobC8yI6g) | Review stream options in a Snort 2 NAP, check cluster health first and decide the TCP MSS and sequence randomization settings |
| [m14-09-snort2-portscan-and-rate-based-prevention](labs/m14-09-snort2-portscan-and-rate-based-prevention/) | [Cisco FMC & FTD: Snort 2: Portscan Detection and Rate-Based Attack Prevention](https://youtu.be/xvooPeKRnXc) | Enable portscan detection with a chosen sensitivity, turn on GID 122 rules and add rate-based prevention with thresholds from a measured baseline |
| [m14-10-adaptive-profiles-and-host-context](labs/m14-10-adaptive-profiles-and-host-context/) | [Cisco FMC & FTD: Adaptive Profiles and Host Context for Inspection](https://youtu.be/RKzK_HZmPnA) | Check network discovery data, enable adaptive profiles and profile updates in the access control policy and compare events before and after |

More labs will be added folder by folder, following the video order.

## How the labs are written

- The steps follow the video and the official Cisco Secure Firewall Management Center
  Device Configuration Guide. Always confirm behavior against the guide for your exact
  FMC/FTD version.
- Labs are outlines you can follow on your own equipment. Menu names can differ between
  versions, so the guide chapter is referenced in each lab.

## Want the full lesson notes?

The [FMC & FTD Study Pack](https://whop.com/nizar-tuanku/fmc-ftd-study-pack/?utm_source=github&utm_medium=readme&utm_campaign=labs)
adds the complete notes, worked scenarios and self-check quizzes for every lesson. The labs
in this repository stay free.

## Feedback

Found a mistake or something unclear? Please open an issue.

## License

Apache License 2.0, see [LICENSE](LICENSE).

*Independent training by Hexward Labs. Not affiliated with or endorsed by Cisco Systems.*
