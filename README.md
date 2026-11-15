# Awesome-Managed-Service-Provider-MSP-ITSM

# Awesome Managed Service Provider (MSP) ITSM

> A curated list of top Managed Service Provider (MSP) ITSM and PSA platforms — both SaaS/Hosted commercial solutions and open-source alternatives for ticketing, client management, billing, and remote monitoring.
> 🌟 Star this repo if you find it useful! 🌟

---

## 📋 Table of Contents

- [SaaS / Hosted Platforms](#-saas--hosted-platforms)
  - [ConnectWise Manage](#connectwise-manage)
  - [Datto Autotask PSA](#datto-autotask-psa)
  - [Kaseya BMS](#kaseya-bms)
  - [HaloPSA](#halopsa)
  - [Syncro MSP](#syncro-msp)
  - [Atera](#atera)
  - [SuperOps.ai](#superopsai)
- [Open-Source Software](#-open-source-software)
  - [AlgaPSA](#algapsa)
  - [ClientSt0r](#clientst0r)
  - [LightPSA](#lightpsa)
  - [ITFlow](#itflow)
  - [iTop](#itop)
  - [NetLock RMM](#netlock-rmm)

---

## 🟦 SaaS / Hosted Platforms

Commercial, cloud-hosted MSP ITSM and PSA platforms. These are not open-source but are included as reference points for feature comparison.

### ConnectWise Manage
**Type:** Comprehensive PSA for MSPs
ConnectWise Manage is the long-standing enterprise standard for MSP professional services automation, covering help desk, project management, billing, procurement, and client management. It is positioned for established MSPs with complex operations, with pricing that reflects its enterprise focus.

### Datto Autotask PSA
**Type:** Cloud PSA with RMM integration
Datto Autotask PSA provides ticketing, project management, time tracking, billing, and CRM for MSPs, tightly integrated with Datto RMM and the broader Kaseya ecosystem. It is positioned for mid-market MSPs wanting a unified PSA and RMM stack.

### Kaseya BMS
**Type:** Cloud business management for MSPs
Kaseya BMS provides help desk, CRM, billing, and project management for MSPs, integrated with Kaseya VSA for remote monitoring. It is positioned for MSPs already using Kaseya tools.

### HaloPSA
**Type:** Modern PSA with ITSM and ITIL alignment
HaloPSA provides a modern, ITIL-aligned PSA platform with ticketing, asset management, SLAs, and reporting. It is positioned for MSPs wanting a cleaner interface and stronger ITIL alignment than legacy PSA tools.

### Syncro MSP
**Type:** All-in-one MSP platform with RMM and PSA
Syncro combines PSA, RMM, and remote access in a single platform with flat-rate per-technician pricing. It is positioned for smaller MSPs wanting an integrated stack without per-device fees.

### Atera
**Type:** RMM and PSA with per-technician pricing
Atera provides RMM, PSA, and remote access with per-technician pricing rather than per-device, making it predictable for MSPs managing many endpoints. It is positioned for MSPs and IT teams wanting an all-in-one platform.

### SuperOps.ai
**Type:** Modern MSP platform with AI assistance
SuperOps.ai provides PSA and RMM with AI-powered assistance for ticket triage, documentation, and automation. It is positioned for MSPs wanting a modern, AI-native platform.

---

## 🟩 Open-Source Software

Self-hosted, community-driven MSP ITSM and PSA tools. The open-source ecosystem is **growing**, with several projects explicitly targeting MSP workflows.

### AlgaPSA
**Stack:** Next.js / TypeScript / PostgreSQL / Redis | **License:** AGPL-3.0 (Community Edition) 
AlgaPSA is a professional services automation platform built specifically for Managed Service Providers, bringing client records, service tickets, time tracking, contracts, billing, invoicing, documents, assets, reporting, and automation into one MSP-focused system . Key capabilities include:
- **Service desk and client operations**: Support ticketing, client/contact/company management, multilingual client portal, document management with version control, asset management, and project/task management 
- **Time, contracts, and billing**: Time tracking with approval workflows, automatic interval tracking for ticket work stored in IndexedDB, flexible billing cycles (weekly, bi-weekly, monthly, quarterly), proration support, contract purchase orders, sales quotes, and a graphical invoice/quote designer for branded PDFs 
- **Automation and reporting**: Workflow Automation with an Event Catalog for ticket, billing, scheduling, email, and CRM triggers; visual workflow designer; Redis-backed event processing; RBAC and ABAC; API and extension SDK 
- **International tax support**: Composite rates, thresholds, tax holidays, and reverse charge scenarios 

The Community Edition is the self-hostable AGPL core, with an Enterprise Edition path for commercially licensed modules and larger deployments . The platform is built by Nine Minds, founded by a former ConnectWise Chief Architect with 17 years of industry experience .  
**Best for:** MSPs wanting a modern, self-hostable PSA with strong billing and contract workflows, accepting the AGPL licensing for the Community Edition.

### ClientSt0r
**Stack:** Django 6 / MariaDB / Docker | **License:** MIT 
ClientSt0r is self-hosted IT documentation and service desk software for MSPs and IT teams, keeping client documentation, assets, credentials, and support work in one structured, searchable system . Key capabilities include:
- **Documentation and knowledge base**: Client documentation, runbooks, and internal knowledge base with owners, review dates, drafts, and version history; documentation readiness scoring per client with a repair queue 
- **Asset and credential management**: Asset tracking, rack elevations, warranty/lifecycle dates, and an AES-256-GCM encrypted credential vault with audited reveals 
- **Service desk (opt-in)**: Tickets, SLAs, contracts, quotes, and invoices, with a My Work page for each technician 
- **Client portal**: Clients see only tickets shared with them and can request services through guided forms 
- **Security**: Azure AD/Entra ID SSO and LDAP/AD sign-in, Content-Security-Policy with per-request nonces, CodeQL and dependency scanning 

It is MIT-licensed with every first-party feature free and unrestricted when self-hosted—no paid tiers, no seat or client limits, and no licence activation . Optional managed hosting and commercial support are offered separately.  
**Best for:** MSPs wanting self-hosted documentation and service desk with no feature gating, accepting the Django/MariaDB stack.

### LightPSA
**Stack:** Next.js / Prisma / PostgreSQL | **License:** Open Source (GitHub) 
LightPSA is a PSA and ticketing system for MSPs with a modern web interface . Key capabilities include:
- **Ticketing**: Filterable queues across boards and clients, ticket detail with time logs, comments, canned responses, SLA countdown, and properties 
- **Client and asset management**: Companies with parent/child accounts, contacts with portal access, assets (servers, network devices, workstations) tracked per client 
- **Billing and SLAs**: Approve and lock billable time/expenses before invoicing, SLA policies with response/resolution targets per priority 
- **Automation and reporting**: IFTTT-style automation rules (triggers, conditions, actions), reports for ticket volume, SLA compliance, and technician utilization 
- **Client portal**: Contacts see only their own company's tickets and public KB articles 

Deploys via Docker Compose (`docker compose up -d`), with demo data and login credentials provided .  
**Best for:** MSPs wanting a modern, self-hosted PSA with a clean interface and Docker deployment, accepting a newer project than AlgaPSA.

### ITFlow
**Stack:** (Check repository) | **License:** Open Source 
ITFlow is an open-source Professional Services Automation platform designed for MSPs, IT consultants, and internal IT teams . Key features include:
- **Client and contact management**
- **Integrated help desk and ticketing**
- **Asset inventory and lifecycle management**
- **Secure documentation and credential management**
- **Project and task management**
- **Invoicing, billing, expense tracking, and financial reporting**
- **Client portal** for accessing tickets, invoices, and documentation 
- **Role-based access controls and user permission management**
- **Business reporting and operational analytics**

It is self-hosted with full data ownership and multi-client management capabilities . The project has **1,005 GitHub stars** and is actively updated (last update within the week as of the source data) .  
**Best for:** MSPs wanting a comprehensive open-source PSA with asset, billing, and documentation features, accepting a larger, established project.

### iTop
**Stack:** PHP / MySQL | **License:** AGPL-3.0 
iTop (IT Operations Portal) is a complete open-source, web-based IT service management platform, including a fully customizable CMDB, helpdesk system, and document management tool . It is ITIL compliant and easily customizable and extensible through add-ons and web services . Key features include:
- **Fully configurable Configuration Management (CMDB)**
- **HelpDesk and Incident Management**
- **Service and Contract Management**
- **Change Management**
- **Configurable SLA Management**
- **Graphical impact analysis**
- **CSV import tool** for any data 
- **Consistency audit** to check data quality 
- **Data synchronization** for data federation 

iTop development is sponsored, led, and supported by Combodo .  
**Best for:** MSPs and IT teams wanting a proven, ITIL-compliant ITSM platform with CMDB and contract management, accepting the PHP/MySQL deployment.

### NetLock RMM
**Stack:** C# / .NET / Blazor / MySQL | **License:** Open Core (Community up to 25 devices) 
NetLock RMM is an open-core remote monitoring and management platform from Germany, positioned for MSPs and enterprises . Key capabilities include:
- **Application Control** (Windows): In-house default-deny allowlisting engine matching path, version info, SHA256/SHA512 hashes, and certificate details 
- **USB Device Control** (Windows): Allowlist devices by vendor ID, product ID, serial, or device class 
- **Antivirus & Firewall**: Manage Microsoft Defender Antivirus, monitor firewall status, and drive Linux UFW Firewall Manager 
- **Ticketing, Helpdesk & CRM**: Optional helpdesk module with multi-department IMAP/SMTP, SLA engine, time tracking (auto + manual, billable rounding), native CRM with tenant linkage 
- **Reports**: 53 pre-built templates plus a visual query builder and raw-SQL "God Mode" 
- **NetLock AI**: OpenAI-API-compatible LLM connector (OpenAI, Claude, or self-hosted models) wired into the script editor, remote shell, event-log viewer, ticketing, and auditing 
- **White-Label Branding**: Theme every colour, logo, and title; brand the tray icon, support chat, and screen-control prompts 
- **Security**: Agent handshake, Trust Server supply-chain hash verification, RAM-based encrypted package delivery, outbound-only agents, end-to-end encryption for relay connections, no hidden telemetry 

The Community Edition is self-hosted and supports up to **25 devices**, with all core features and code-signed Windows agents included .  
**Best for:** Small MSPs and homelabs wanting a modern, secure RMM with helpdesk and CRM capabilities up to 25 devices, accepting the open-core model for larger deployments.

---

## 📊 Comparison at a Glance

| Software | License | Stack | Ticketing | Billing | RMM | Self-Hosted | Best For |
|----------|---------|-------|-----------|---------|-----|-------------|----------|
| **ConnectWise** | Proprietary | Cloud | ✅ | ✅ | (Separate) | ❌ | Enterprise MSPs |
| **Autotask** | Proprietary | Cloud | ✅ | ✅ | (Datto RMM) | ❌ | Mid-market PSA + RMM |
| **HaloPSA** | Proprietary | Cloud | ✅ | ✅ | (Separate) | ❌ | Modern ITIL-aligned PSA |
| **Atera** | Proprietary | Cloud | ✅ | ✅ | ✅ | ❌ | Per-technician pricing |
| **AlgaPSA** | AGPL-3.0 | Next.js/Postgres | ✅ | ✅ Deep | ❌ | ✅ | Self-hosted PSA + billing |
| **ClientSt0r** | MIT | Django/MariaDB | ✅ | ✅ | ❌ | ✅ | Self-hosted docs + service desk |
| **LightPSA** | Open Source | Next.js/Postgres | ✅ | ✅ | ❌ | ✅ | Modern self-hosted PSA |
| **ITFlow** | Open Source | (Check) | ✅ | ✅ | ❌ | ✅ | Comprehensive OSS PSA |
| **iTop** | AGPL-3.0 | PHP/MySQL | ✅ | ✅ Contracts | ❌ | ✅ | ITIL ITSM + CMDB |
| **NetLock RMM** | Open Core | C#/.NET/MySQL | ✅ | (Check) | ✅ | ✅ | Secure RMM up to 25 devices |

---

## 🤝 Contributing

Contributions are welcome! If you know of an open-source MSP ITSM or PSA tool that should be listed here, please open a pull request with:

- Project name and URL
- Brief description (1–2 sentences)
- Stack and license
- Why it stands out

Please ensure the project is actively maintained (releases within the last 12 months) and genuinely open-source.

**Note on the open-source ecosystem:** The open-source MSP ITSM and PSA space has matured significantly in 2026. **AlgaPSA** is the most comprehensive open-source PSA, built by a former ConnectWise Chief Architect, with deep billing and contract workflows . **ClientSt0r** is the strongest MIT-licensed option for documentation and service desk, with no feature gating . **LightPSA** offers a modern Next.js/PostgreSQL alternative, and **ITFlow** provides a comprehensive, established PSA with 1,000+ GitHub stars . **iTop** remains the best choice for organizations needing ITIL-compliant ITSM with a CMDB . For RMM specifically, **NetLock RMM** offers a secure, open-core platform with helpdesk and CRM included up to 25 devices . No single open-source project fully replicates ConnectWise's enterprise breadth, but these tools cover the core MSP workflows—ticketing, billing, documentation, and RMM—for self-hosted deployments.

---

## 📄 License

This list is released under CC0 1.0 Universal (Public Domain). The software projects listed retain their respective licenses.

---

⭐ **If this list helped you discover a useful tool, please star the repo!** ⭐
