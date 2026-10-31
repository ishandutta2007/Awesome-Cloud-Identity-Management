# Awesome-Cloud-Identity-Management

# Awesome-Cloud-Identity-Management

**Top Cloud Identity Management (Opensource) 🌟 Star if you like it! 🌟**



**Curated List of SaaS Products & Open-Source GitHub Projects**

*Focused on SSO, MFA, Identity Governance, Passwordless Authentication & Self-Hosted IAM*

**Last updated: October 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Cloud Identity Management**. These tools enable organizations to authenticate users, enforce access policies, manage identities across applications, and govern entitlements—from fully managed enterprise IAM platforms with AI-driven risk scoring to self-hosted identity providers that give teams complete control over their user directory and authentication flows.



**Examples** include Microsoft Entra ID, Okta, Ping Identity, CyberArk Identity, OneLogin, Auth0, JumpCloud, ForgeRock, and Beyond Identity (the category leaders in commercial space).



**Open-source emphasis**: This section is expanded with every relevant project for self-hosted IAM, SSO, and open identity infrastructure. **Critical note**: The open-source IAM landscape is exceptionally mature—**Keycloak** remains the most widely deployed, but **Casdoor** has emerged as the most feature-complete modern alternative with built-in MCP server and AI-agent support, while **Zitadel** and **Authentik** offer cloud-native and community-favorite options respectively. No open-source project matches Okta's or Microsoft Entra's breadth of pre-built application integrations and governance features out of the box, but for core authentication and SSO, the open-source options are production-proven at scale.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[Microsoft Entra ID](https://www.microsoft.com/en-us/security/business/identity-access/microsoft-entra-id)**

  **Cloud identity and access management** integrated with Microsoft 365 and Azure. Ranked as the **overall leader** in ISG's 2026 Identity and Access Management Platforms Buyers Guide, with top scores in five categories including Product Experience and Customer Experience . **Pricing**: Included with Microsoft 365 plans; Premium P1/P2 add-ons for advanced governance and identity protection. **Free tier**: Limited free tier available. **Best for**: Microsoft-centric organizations wanting native integration with Teams, Outlook, and Azure resources—**trade-off**: ecosystem lock-in and licensing complexity.



- **[Okta](https://www.okta.com/)**

  **Enterprise identity platform** with broad application integrations and adaptive MFA. Named a **Leader** in Product Experience in ISG's 2026 Buyers Guide, alongside Microsoft and AWS . **Pricing**: Quote-only; per-user and per-application models. **Free tier**: Developer edition available. **Best for**: large enterprises needing vendor-neutral IAM across a diverse application portfolio—**trade-off**: premium pricing and configuration complexity.



- **[Ping Identity](https://www.pingidentity.com/)**

  **Identity and access management** for workforce and customer identity, with AI-driven fraud protection (via ForgeRock merger). Rated **Innovative** in ISG's 2026 Buyers Guide . Offers PingOne for Customers (from ~$35K/year) and PingOne for Workforce (from ~$3/user/month, 5,000-user minimum) . **Pricing**: Quote-only; tiered by customer vs. workforce and volume. **Free tier**: None. **Best for**: organizations needing advanced fraud protection and AI-driven access decisions—**trade-off**: pricing not designed for small businesses .



- **[CyberArk Identity](https://www.cyberark.com/)**

  **Identity security platform** with privileged access management and adaptive authentication. Rated **Exemplary** in ISG's 2026 Buyers Guide . **Pricing**: Quote-only. **Free tier**: None. **Best for**: enterprises prioritizing privileged access security and identity threat detection.



- **[OneLogin](https://www.onelogin.com/)** (One Identity)

  **Cloud IAM platform** with SSO, MFA, and directory integration. Rated **Exemplary** in ISG's 2026 Buyers Guide . **Pricing**: Quote-only; tiered by users. **Free tier**: Trial available. **Best for**: mid-market organizations wanting straightforward SSO and MFA—**trade-off**: less extensive governance features than Okta or Entra.



- **[Auth0](https://auth0.com/)** (Okta)

  **Developer-friendly identity platform** for customer-facing applications. **Pricing**: Free tier for small projects; paid plans scale by monthly active users. **Free tier**: Yes, generous for development. **Best for**: developers building applications needing drop-in authentication with social logins, MFA, and RBAC—**trade-off**: customer identity focus, not workforce IAM.



- **[JumpCloud](https://jumpcloud.com/)**

  **Directory platform** combining identity, access, and device management across cloud and on-premise resources. Rated **Assurance** in ISG's 2026 Buyers Guide, but recognized as **best overall IAM solution for 2026** in eSecurity Planet's evaluation for combining identity, directory, and cross-platform device management . **Pricing**: Tiered per-user pricing; free tier for small teams. **Free tier**: Yes, up to 10 users. **Best for**: IT teams wanting unified directory for identity and device management without Active Directory.



- **[ForgeRock](https://www.forgerock.com/)** (Ping Identity)

  **Enterprise IAM platform** with AI-driven identity governance and fraud protection, now merged with Ping Identity . **Pricing**: Bundled with Ping Identity offerings. **Free tier**: None. **Best for**: organizations needing advanced identity governance and AI-powered risk assessment—**trade-off**: enterprise pricing and complexity.



- **[Atlassian Identity](https://www.atlassian.com/)**

  **Native identity management** for Atlassian Cloud products (Jira, Confluence, etc.). **Pricing**: Included with Atlassian subscriptions; Atlassian Guard for advanced security. **Free tier**: Limited. **Best for**: Atlassian customers wanting user provisioning and SSO within the Atlassian ecosystem—**not** a general-purpose IAM platform.



- **[Beyond Identity](https://www.beyondidentity.com/)**

  **Passwordless identity platform** with device-bound credentials. Rated **Merit** in ISG's 2026 Buyers Guide . **Pricing**: Quote-only. **Free tier**: Developer tier available. **Best for**: organizations eliminating passwords entirely with phishing-resistant authentication.



## Open-Source GitHub Projects



- **[Casdoor](https://github.com/casdoor/casdoor)**

  **AI-native Identity and Access Management (IAM) / SSO platform with web UI** (Apache-2.0) — **the most feature-complete modern open-source IAM platform** as of October 2026, with built-in support for protocols that others require extensions to achieve . **Features**: **OAuth 2.0 / OIDC provider**, **SAML 2.0 IdP**, **CAS server** (built-in), **LDAP server** (built-in), **RADIUS server** (built-in), **WebAuthn / passkeys**, **TOTP / MFA**, **Face ID** biometric sign-in . **MCP server and OAuth 2.1 for MCP built in**—the only self-hosted IdP with native Model Context Protocol support, enabling AI agents to authenticate and access resources . **SCIM 2.0 server** for receiving users from Entra ID/Okta; **syncers for Keycloak, Okta, Entra ID, Active Directory, Google Workspace, AWS IAM**, and more . **Casbin policy engine** for ACL, RBAC, ABAC, and custom authorization models . **70+ built-in social/enterprise providers** including WeChat, DingTalk, Lark, and Alipay . **Multi-tenancy** via Organizations with isolated users, applications, and branding. **Everything editable in the UI**—no file redeployment needed. **Single Go binary** plus database; no JVM, no operator, no cluster required . **Tech stack**: Go (backend), React (UI). **Deploy**: Docker all-in-one for evaluation; Docker Compose with MySQL for production; Casdoor Cloud for managed . **Trade-off**: **Smaller community than Keycloak**—fewer third-party tutorials and Stack Overflow answers. Documentation is improving but less comprehensive than Keycloak's ecosystem . **Best for**: teams wanting the broadest protocol support (including MCP for AI agents) in a modern, UI-first self-hosted IAM platform—especially those building AI-integrated applications or needing built-in CAS/LDAP/RADIUS without extensions.



- **[Keycloak](https://github.com/keycloak/keycloak)**

  **Open Source Identity and Access Management** (Apache-2.0) — **the most widely deployed open-source IAM platform**, with the largest ecosystem and community. **Features**: OAuth 2.0/OIDC, SAML 2.0, LDAP/AD federation, social login (about a dozen built-in plus generic OIDC/SAML), user federation and live LDAP lookups, authentication flows with Java SPI extension points, realm import, and SCIM 2.0 server support (since 26.8) . **Tech stack**: Java (Quarkus). **Deploy**: Self-hosted (Operator for Kubernetes, Docker) or managed via Red Hat build. **Trade-off**: **Java overhead is real**—heavier footprint and slower startup than Go-based alternatives . **UI is clunky and user self-service is an afterthought**—the community recommends Authentik for better user experience . **Rated Merit in ISG's 2026 Buyers Guide** . **Best for**: organizations needing a proven, battle-tested IAM with the largest ecosystem—willing to accept Java overhead and a dated UI in exchange for maximum community support and third-party integrations.



- **[Zitadel](https://github.com/zitadel/zitadel)**

  **Cloud-native identity management platform** (AGPL-3.0) — **the most resource-efficient and Kubernetes-native open-source IAM**, written in Go for fast startup and low memory footprint . **Features**: OIDC, OAuth2, SAML 2.0; **multi-tenancy via Instances and Organizations**—clean isolation for external project members or freelancers as separate identity populations ; **self-service portal** for users to manage credentials and MFA; **API-first design** for extensibility without the Java ecosystem. **Tech stack**: Go, TypeScript (login UI), PostgreSQL. **Deploy**: Self-hosted (Helm chart, Kubernetes). **Trade-off**: **Newer and smaller community than Keycloak**—documentation is good but less comprehensive . **Best for**: small businesses and platform teams deploying in containerized/Kubernetes environments where resource efficiency matters—especially those managing external users or contractors as separate tenants.



- **[Authentik](https://github.com/goauthentik/authentik)**

  **Modern open-source identity provider** (MIT core, enterprise features commercial) — **the community favorite for Keycloak migration**, with a clean modern UI and out-of-the-box user self-service portal . **Features**: SAML, OAuth2, OIDC; **most flexible sign-in flow engine** among the four major self-hosted IdPs—flows and stages edited in the admin interface ; **user-facing portal** for profile management, password reset, and MFA device configuration without admin intervention ; **proxy provider** for Traefik, Caddy, Nginx, and Envoy with headers set by outpost; **LDAP source** sync and password checks; **SCIM source** for receiving users. **Tech stack**: Python/Django and Go. **Deploy**: Self-hosted (Helm chart, Docker). **Trade-off**: **Not as lightweight as Zitadel**—Python/Django backend means heavier resource usage, though rarely a constraint for small business deployments . **Separate tenants are an alpha enterprise feature**—multi-tenancy is via Brands for branding, not full isolation . **Best for**: teams wanting a modern, clean IAM with excellent user self-service and flexible sign-in flows—especially those frustrated by Keycloak's UI and seeking a community-recommended alternative.



- **[Ory (Kratos, Hydra, Keto, Oathkeeper, Polis)](https://github.com/ory)**

  **Modular, cloud-native IAM ecosystem** (Apache-2.0) — **the most architecturally flexible open-source IAM**, with each service solving a distinct problem and working standalone or combined . **Components**: **Ory Kratos** (identities, credentials, sessions, self-service flows—passwords, social sign-in, OIDC, passkeys, MFA); **Ory Hydra** (OpenID Certified® OAuth 2.0 and OIDC provider—token issuance, delegation, stateless JWT); **Ory Keto** (fine-grained permissions—Google Zanzibar model, RBAC/ABAC); **Ory Oathkeeper** (identity and policy-aware zero-trust proxy); **Ory Polis** (SAML to OAuth 2.0 bridge, enterprise SSO) . **Headless architecture**—bring your own UI; **Ory Elements** component library for building custom login/registration/settings flows. **Tech stack**: Go (all services). **Deploy**: Self-hosted (Docker, Kubernetes Helm charts) or Ory Network (managed SaaS). **Trade-off**: **Modular means more assembly required**—you choose and integrate the components you need; not a single monolithic IdP. **Guaranteed CVE patching and SLAs require Ory Enterprise License** . **Best for**: developers and platform teams wanting maximum architectural flexibility—especially those building microservices or needing Zanzibar-style fine-grained permissions alongside authentication.



- **[Janssen Project](https://github.com/JanssenProject/jans)**

  **Linux Foundation-governed open-source IAM** (Apache-2.0) — **the most standards-complete and governance-backed open-source IAM**, recognized as a **Digital Public Good** by the Digital Public Goods Alliance (18/18 checks met) . **Features**: **Jans Auth Server** (certified OpenID Connect Provider, OAuth 2.0 server); **Agama** low-code identity orchestration DSL for authentication journeys; **Jans FIDO** for passkeys and FIDO2; **Jans SCIM** for user management; **Jans Cedarling**—embeddable Rust-based policy decision point with WASM, iOS, Android, and Python bindings; **Jans Lock** for enterprise authorization with centralized audit logs . **Standards**: OAuth 2.0, certified OIDC, SAML 2.0, FIDO2, SCIM, UMA 2.0 . **Tech stack**: Java. **Deploy**: Self-hosted (Helm for Kubernetes, VM packages for Ubuntu/SUSE/Red Hat). **Trade-off**: **Complex deployment**—requires Kubernetes or VM infrastructure; not a simple single-binary install. **Commercial distributions** (Gluu Flex, Gluu Solo) offer support and enterprise features . **Best for**: public sector, regulated industries, and organizations needing a Digital Public Good-certified IAM with Linux Foundation governance and the most complete standards coverage—especially those building national-scale identity infrastructure.



### Additional Strong Open-Source Options



- **Shibboleth Consortium** — Web-based SSO and federated identity (open source). **Note**: **Higher education and research focus**—excels at inter-organizational federation and resource sharing; not a general-purpose workforce IAM . **Best for**: universities and research institutions needing federated authentication across organizations.

- **FreeIPA + Keycloak** — Established self-hosted stack (open source). FreeIPA for directory/Kerberos/SSH keys/certificates; Keycloak for SSO on top. **Note**: **Heavier and more complex**—best when you need the full AD-equivalent feature set (Kerberos, certificate management, HBAC, sudo rules) . **Best for**: organizations needing complete directory services beyond SSO.



**Frameworks for building custom systems**: Combine **Casdoor** for broad protocol support (including MCP for AI agents) with **Zitadel** for Kubernetes-native multi-tenancy, **Authentik** for user self-service and flexible flows, and **Ory Kratos + Keto** for modular identity and Zanzibar-style permissions—creating an IAM stack matched to each team's deployment environment and feature priorities. **None of these match Okta's or Entra's pre-built application catalog**, but for core authentication, SSO, and governance, the open-source options are production-proven at scale.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, license (for open-source), and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- Identity management platforms handling credentials and personal data must comply with data protection regulations (GDPR, CCPA, etc.) and implement appropriate encryption, MFA, and audit logging.

- **The "enterprise IAM platform" vs. "developer-friendly CIAM" vs. "modular IAM ecosystem" vs. "federated SSO" distinction is critical.** **Microsoft Entra ID, Okta, Ping Identity, CyberArk, OneLogin, JumpCloud, ForgeRock, and Atlassian Identity** are **enterprise IAM platforms**—they provide workforce SSO, governance, and broad application integrations. **Auth0** is **developer-friendly CIAM**—optimized for customer-facing applications. **Casdoor, Keycloak, Zitadel, and Authentik** are **self-hosted IAM platforms**—they provide authentication and SSO, but you own infrastructure and integration work. **Ory** is a **modular ecosystem**—you assemble components based on need. **Janssen** is a **standards-complete federated IAM** with Digital Public Good certification. **Shibboleth** is **federated SSO** for research/education. **Choose based on whether you need managed convenience, developer experience, self-hosted control, or federated identity.**

- **Casdoor is the most feature-complete modern open-source IAM** as of October 2026. It is the **only self-hosted IdP with built-in MCP server and OAuth 2.1 for MCP**—critical for AI-agent authentication . It also includes built-in CAS, LDAP, and RADIUS servers that Keycloak and others require extensions to achieve . **The trade-off**: smaller community than Keycloak, with fewer tutorials and Stack Overflow answers.

- **Keycloak remains the ecosystem leader** with the largest community, most third-party integrations, and Red Hat backing. **The trade-off**: Java overhead, dated UI, and poor user self-service experience—the community increasingly recommends Authentik or Zitadel for modern deployments .

- **Authentik is the community favorite for Keycloak migration**, with a clean UI, user self-service portal, and the most flexible sign-in flow engine among self-hosted IdPs . **Zitadel is the Kubernetes-native choice**—Go-based for low resource usage, with clean multi-tenancy for external users/contractors .

- **Ory is the architectural flexibility champion**—modular Go services (Kratos, Hydra, Keto, Oathkeeper, Polis) that can be adopted individually or combined, with a path to Ory Network if you later want managed deployment . **The trade-off**: more assembly required; enterprise SLAs require commercial licensing.

- **Janssen is the governance and standards choice**—Linux Foundation-governed, Digital Public Good certified, with the most complete standards coverage (OAuth, OIDC, SAML, FIDO2, SCIM, UMA) and low-code Agama orchestration . **The trade-off**: complex deployment; best suited for public sector and large-scale identity infrastructure.

- **Pricing opacity varies.** Microsoft Entra ID is included with M365 plans. Ping Identity publishes tiered pricing for PingOne (Customers from $35K/year; Workforce from $3/user/month) . Okta, CyberArk, OneLogin, JumpCloud (enterprise), ForgeRock, and Beyond Identity require sales contact. Auth0 has a free tier; JumpCloud has a free tier for up to 10 users. **Validate with direct vendor conversations against your user count and feature requirements.**

- Self-hosted open-source solutions require proper infrastructure (databases, Kubernetes for some), security hardening for authentication endpoints, and ongoing maintenance. **IAM systems are the keys to your kingdom**—ensure your deployment includes MFA enforcement, audit logging, and regular security patching before trusting it with production identities.



---



**Made for identity architects, security teams, and organizations building transparent cloud identity management solutions.**

Let's make Cloud Identity Management more open, data-driven, and passwordless-ready.
