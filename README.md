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
