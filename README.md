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
| [m07-01-identity-from-ip-to-user](labs/m07-01-identity-from-ip-to-user/) | [Identity-Based Policies: Why IP Addresses Alone Are Not Enough](https://youtu.be/KFklKLNshSg) | Turn IP addresses into users with a realm, an identity policy, decryption and a group-based access rule |
| [m07-02-ldap-ad-realms-and-sequences](labs/m07-02-ldap-ad-realms-and-sequences/) | [LDAP/AD Realms, Realm Sequences, and Troubleshooting](https://youtu.be/2T4nDKTXR5U) | Build a realm, encrypt the directory connection, create a realm sequence and learn the failure messages |
| [m07-03-azure-ad-saml-realm](labs/m07-03-azure-ad-saml-realm/) | [Microsoft Azure AD Realms in the SAML Context](https://youtu.be/3fGXzAuIIyk) | Map Microsoft Entra ID identities to firewall access control with a Microsoft Azure AD (SAML) realm |
| [m07-04-passive-identity-agent](labs/m07-04-passive-identity-agent/) | [Passive Identity Agent: Recognizing Users Without a Login Portal](https://youtu.be/ioKDqCbZGgE) | Install a passive identity agent, map logons to IP addresses and test a secondary agent |
| [m07-05-cisco-ise-identity-source](labs/m07-05-cisco-ise-identity-source/) | [Integrating Cisco ISE or ISE-PIC](https://youtu.be/jvftEmY0c2o) | Integrate a lab Cisco ISE node, use SGTs as source and destination conditions, and learn when SXP matters |
| [m07-08-building-identity-policies](labs/m07-08-building-identity-policies/) | [Building and Verifying Identity Policies](https://youtu.be/EsXA-S-EAkk) | Build an identity policy with passive and active rules, handle special identities and prove the association matters |
| [m07-09-zero-trust-application-access](labs/m07-09-zero-trust-application-access/) | [Zero Trust Access: Application Access and Connection Evaluation](https://youtu.be/W7tDtA2p-Lo) | Publish one web application behind the firewall with a Zero Trust Application policy and a SAML identity provider |

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
