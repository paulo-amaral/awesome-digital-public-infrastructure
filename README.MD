# Awesome Digital Public Infrastructure [![Awesome](https://awesome.re/badge.svg)](https://awesome.re) [![Contributions Welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg)](CONTRIBUTING.md) [![GitHub Stars](https://img.shields.io/github/stars/YOUR_USERNAME/awesome-digital-public-infrastructure?style=social)](../../stargazers) [![Last Updated](https://img.shields.io/github/last-commit/YOUR_USERNAME/awesome-digital-public-infrastructure)](../../commits/main)

> **A curated list of Digital Public Infrastructure (DPI) and Digital Public Goods (DPG) — open-source solutions, frameworks, country stacks, and resources for governments, UN agencies, NGOs, and developers building the next generation of inclusive digital societies.**

**Digital Public Infrastructure (DPI)** refers to shared digital systems — identity, payments, data exchange — that are open, interoperable, and reusable by governments and the private sector alike. **Digital Public Goods (DPGs)** are open-source software, data, AI models, and content standards that advance the UN Sustainable Development Goals.

> 🌍 Curated with field experience from UNICEF, UNDP, and real implementations across Asia, the Pacific, and fragile states.  
> If this list helped you, please ⭐ **star the repo** and share with your network.

---

## Contents

- [Why DPI Matters](#why-dpi-matters)
- [Frameworks & Standards](#frameworks--standards)
- [Certified DPGs by Domain](#certified-dpgs-by-domain)
  - [Health](#health)
  - [Identity & Civil Registration](#identity--civil-registration)
  - [Payments & Financial Inclusion](#payments--financial-inclusion)
  - [Education](#education)
  - [Climate & Environment](#climate--environment)
  - [Data Exchange & Interoperability](#data-exchange--interoperability)
  - [Child Protection & Social Protection](#child-protection--social-protection)
- [Country DPI Stacks](#country-dpi-stacks)
- [Toolkits & Assessment Frameworks](#toolkits--assessment-frameworks)
- [Organizations & Communities](#organizations--communities)
- [Research & Reports](#research--reports)
- [Courses & Learning](#courses--learning)
- [Jobs & Opportunities](#jobs--opportunities)
- [🏕️ Field Notes — Real Implementation Insights](#field-notes--real-implementation-insights)
- [Contributing](#contributing)

---

## Why DPI Matters

> *"DPI is to the digital economy what roads, electricity, and water are to the physical economy."*  
> — Co-Develop Fund

DPI enables countries to:
- **Deliver services at scale** — India's UPI processes 10B+ monthly transactions
- **Include the excluded** — MOSIP enables foundational ID for populations without documents
- **Build once, use many times** — Open, interoperable infrastructure avoids vendor lock-in
- **Accelerate the SDGs** — DPGs reduce the cost of digital transformation by up to 90%

As of 2025, **over 50 countries** are actively building or scaling DPI components. The DPG ecosystem counts **140+ certified solutions** across health, education, identity, payments, and climate.

---

## Frameworks & Standards

> Authoritative frameworks that define and guide DPI/DPG development at national and global levels.

- [UNDP Digital Public Goods Standard](https://digitalpublicgoods.net/standard/) — Nine-indicator standard for certifying open-source solutions as Digital Public Goods.
- [GovStack Reference Architecture](https://www.govstack.global/our-work/technical-specifications/) — Building-block approach for assembling government digital services.
- [ITU Digital Transformation Framework](https://www.itu.int/en/ITU-D/Pages/default.aspx) — ITU guidelines and metrics for national digital transformation.
- [OECD Digital Government Policy Framework](https://www.oecd.org/governance/digital-government/oecd-digital-government-policy-framework.htm) — Six dimensions for assessing digital government maturity.
- [World Bank DPI Framework](https://www.worldbank.org/en/topic/digitaldevelopment) — Policy and investment guidance for national digital infrastructure.
- [Co-Develop DPI Framework](https://www.co-develop.net/) — Practical guidance for countries designing sovereign, inclusive DPI.
- [Principles for Digital Development](https://digitalprinciples.org/) — Nine principles adopted by 300+ organizations for technology in development contexts.
- [DPI Safeguards Framework](https://www.co-develop.net/dpi-safeguards) — Rights-based safeguards for DPI design and deployment.

---

## Certified DPGs by Domain

> Software certified by the [Digital Public Goods Alliance](https://digitalpublicgoods.net/) as open-source Digital Public Goods. All solutions listed are openly licensed and advance at least one SDG.

### Health

| Solution | Description | Countries | License |
|----------|-------------|-----------|---------|
| [DHIS2](https://dhis2.org/) | Health information management system — the global standard | 100+ | BSD |
| [OpenMRS](https://openmrs.org/) | Open medical record system for resource-constrained settings | 40+ | MPL 2.0 |
| [OpenHIM](http://openhim.org/) | Health interoperability middleware — openHIE reference implementation | — | MPL 2.0 |
| [iHRIS](https://www.ihris.org/) | Health workforce management and planning system | 20+ | GPL 3.0 |
| [Bahmni](https://www.bahmni.org/) | Hospital information system for low-resource settings | 50+ | AGPL 3.0 |
| [OpenELIS](https://openelis-global.org/) | Laboratory information system for public health labs | — | MPL 2.0 |

### Identity & Civil Registration

| Solution | Description | Countries | License |
|----------|-------------|-----------|---------|
| [MOSIP](https://mosip.io/) | Modular Open Source Identity Platform — foundational national ID | 10+ | MPL 2.0 |
| [OpenCRVS](https://www.opencrvs.org/) | Civil registration and vital statistics — births, deaths, marriages | 10+ | MPL 2.0 |
| [OpenSPP](https://openspp.org/) | Social protection platform built on DPI principles | — | LGPL 3.0 |
| [OpenG2P](https://openg2p.org/) | Government-to-person benefit delivery infrastructure | — | MPL 2.0 |

### Payments & Financial Inclusion

| Solution | Description | Countries | License |
|----------|-------------|-----------|---------|
| [Mojaloop](https://mojaloop.io/) | Open-source payment platform designed for financial inclusion | 10+ | Apache 2.0 |
| [OpenG2P](https://openg2p.org/) | G2P payment infrastructure — vouchers, cash transfers, social benefits | — | MPL 2.0 |
| [Mifos X](https://mifos.org/) | Core banking platform for microfinance institutions | 30+ | MPL 2.0 |
| [Apache Fineract](https://fineract.apache.org/) | Open core banking platform for financial services providers | — | Apache 2.0 |

### Education

| Solution | Description | Users | License |
|----------|-------------|-------|---------|
| [Moodle](https://moodle.org/) | World's most deployed learning management system | 300M+ | GPL 3.0 |
| [H5P](https://h5p.org/) | Interactive HTML5 content and applications for learning | — | MIT |
| [Kolibri](https://learningequality.org/kolibri/) | Offline-capable education platform for underserved communities | — | MIT |
| [OpenEDX](https://openedx.org/) | Open-source platform powering edX and 100+ national deployments | — | AGPL 3.0 |
| [Sunbird](https://sunbird.org/) | National digital infrastructure for learning (India's DIKSHA) | 250M+ | MIT |

### Climate & Environment

| Solution | Description | License |
|----------|-------------|---------|
| [OpenClimate](https://openclimate.network/) | Open data infrastructure for climate action transparency | Apache 2.0 |
| [SEPAL](https://sepal.io/) | FAO platform for geospatial analysis and forest monitoring | MIT |
| [ODK / OpenDataKit](https://getodk.org/) | Mobile data collection for field monitoring and reporting | Apache 2.0 |

### Data Exchange & Interoperability

| Solution | Description | License |
|----------|-------------|---------|
| [X-Road](https://x-road.global/) | Data exchange layer — backbone of Estonia's e-government | MIT |
| [OpenHIE](https://ohie.org/) | Health information exchange architecture and community | — |
| [FHIR (HL7)](https://hl7.org/fhir/) | Global standard for healthcare data exchange and interoperability | — |
| [KoboToolbox](https://www.kobotoolbox.org/) | Data collection platform for humanitarian and development contexts | GPL |
| [CommCare](https://www.dimagi.com/commcare/) | Mobile data collection for frontline health and social workers | Apache 2.0 |

### Child Protection & Social Protection

| Solution | Description | License |
|----------|-------------|---------|
| [Primero](https://www.primero.org/) | Child protection case management (UNICEF, UNHCR, IRC) | AGPL 3.0 |
| [RapidPro](https://app.rapidpro.io/) | Messaging platform for humanitarian and development programs | AGPL 3.0 |
| [CPIMS+](https://www.cpimsglobal.org/) | Child protection information management system | AGPL 3.0 |
| [OpenSRP](https://smartregister.org/) | Smart register platform for community health workers | Apache 2.0 |

---

## Country DPI Stacks

> Real-world national implementations. Each profile covers DPI components deployed, key challenges, lessons learned, and open-source tools in use.

| Country | Population | DPI Highlights | Status |
|---------|------------|----------------|--------|
| 🇮🇳 India | 1.4B | Aadhaar (ID), UPI (Payments), ONDC (Commerce), DigiLocker, ABDM (Health) | [View Profile →](docs/country-profiles/india.md) |
| 🇪🇪 Estonia | 1.4M | X-Road (Data Exchange), e-Residency, KSI Blockchain, i-Voting | [View Profile →](docs/country-profiles/estonia.md) |
| 🇧🇷 Brazil | 215M | PIX (Payments), GOV.BR (Identity), Open Finance, Conecte SUS (Health) | [View Profile →](docs/country-profiles/brazil.md) |
| 🇹🇱 Timor-Leste | 1.3M | CPMIS (Child Protection), e-SISCA (Health), RDTL Digital Services | [View Profile →](docs/country-profiles/timor-leste.md) |
| 🇰🇪 Kenya | 55M | Huduma Namba (ID), M-Pesa integration, eCitizen portal | *Coming soon* |
| 🇷🇼 Rwanda | 14M | Irembo portal, National ID, Mobile money ecosystem | *Coming soon* |
| 🇵🇭 Philippines | 115M | PhilSys (ID), InstaPay, eGovPH portal | *Coming soon* |
| 🇸🇳 Senegal | 17M | Wari, Orange Money, DER digital inclusion programs | *Coming soon* |
| 🇫🇯 Fiji | 900K | Digital Fiji strategy, mHealth pilots | *Coming soon* |

> 💡 **Want to contribute a country profile?** See [CONTRIBUTING.md](CONTRIBUTING.md).

---

## Toolkits & Assessment Frameworks

> Practical tools for planning, assessing, and implementing DPI/DPG.

### Digital Readiness & Assessment
- [ITU ICT Development Index](https://www.itu.int/en/ITU-D/Statistics/Pages/publications/mis/methodology.aspx) — Global benchmark for digital readiness across 167 countries.
- [OECD Digital Government Index](https://www.oecd.org/governance/digital-government/digital-government-index.htm) — Maturity model across 6 dimensions.
- [DIAL Digital Investment Framework](https://digitalimpactalliance.org/research/digital-investment-framework/) — How to assess and prioritize DPG investments.
- [WEF Global Technology Governance Report](https://www.weforum.org/reports/global-technology-governance-report-2021/) — Framework for responsible DPI deployment.
- [GovStack Digital Readiness Assessment](https://www.govstack.global/) — Country readiness tool for building-block-based DPI.

### Interoperability Frameworks
- [GovStack Building Blocks Specification](https://govstack.gitbook.io/specification/) — Technical specs for interoperable government services.
- [OpenHIE Architecture](https://ohie.org/framework/) — Health information exchange reference architecture.
- [IHE Integration Profiles](https://www.ihe.net/resources/profiles/) — Integration profiles for healthcare interoperability.

### Procurement & Policy
- [UNICEF Venture Fund Guidance](https://www.unicef.org/innovation/venturefund) — How to fund and scale DPGs in development contexts.
- [Digital Square Global Goods Maturity Model](https://digitalsquare.org/global-goods-maturity-model) — Maturity framework for health digital tools.
- [Open Source Policy Guide](https://github.com/OpenSourcePolicyCenter/toolkit) — Policy frameworks for government open-source adoption.
- [ITU Model Policy on Open Source](https://www.itu.int/) — ITU guidance for national open source policies.

---

## Organizations & Communities

> Key actors shaping the global DPI/DPG ecosystem.

### UN System & Multilaterals
| Organization | Role |
|---|---|
| [Digital Public Goods Alliance (DPGA)](https://digitalpublicgoods.net/) | Multi-stakeholder body defining and certifying DPGs |
| [UNICEF Office of Innovation](https://www.unicef.org/innovation/) | DPG investment and frontier tech for children |
| [UNDP Digital](https://www.undp.org/digital) | Digital transformation support in 170+ countries |
| [ITU](https://www.itu.int/) | UN specialized agency for ICTs |
| [World Bank Digital Development](https://www.worldbank.org/en/topic/digitaldevelopment) | Financing and TA for digital infrastructure |
| [UN OICT](https://unite.un.org/) | UN Office of Information and Communications Technology |

### Foundations & Alliances
| Organization | Focus |
|---|---|
| [Digital Impact Alliance (DIAL)](https://digitalimpactalliance.org/) | Research and convening on digital development |
| [Digital Square](https://digitalsquare.org/) | Pathfinder Fund for global digital health goods |
| [Co-Develop Fund](https://www.co-develop.net/) | Philanthropic DPI funding for low-income countries |
| [Gates Foundation Digital Financial Services](https://www.gatesfoundation.org/our-work/programs/global-growth-and-opportunity/financial-services-for-the-poor) | Financial inclusion through DPI |
| [Omidyar Network](https://omidyar.com/) | Investment in DPI and open internet |
| [Rockefeller Foundation](https://www.rockefellerfoundation.org/) | Digital equity and inclusive DPI |

### Technical Communities
- [GovStack Community](https://www.govstack.global/) — Technical community for reusable government building blocks.
- [OpenHIE Community](https://ohie.org/) — Global health information exchange implementers.
- [Digital Development Forum](https://www.digitaldevelopment.org/) — Community of practice for ICT4D practitioners.
- [ICTworks](https://www.ictworks.org/) — Knowledge hub for digital development professionals.

---

## Research & Reports

> Foundational papers, impact studies, and policy briefs. Sorted by relevance.

### Must-Read: Foundational
- [The Case for a New Digital Bretton Woods](https://www.bu.edu/gdp/files/2022/05/GDP_PB_032_FIN.pdf) — Boston University Global Development Policy Center.
- [DPI: A Moonshot for Equitable Growth](https://www.co-develop.net/dpi-moonshot) — Co-Develop Fund, 2022.
- [Rethinking Digital Public Infrastructure](https://www3.weforum.org/docs/WEF_Rethinking_Digital_Public_Infrastructure.pdf) — World Economic Forum.
- [Digital Public Infrastructure and Democracy](https://www.omidyar.com/insights/) — Omidyar Network.

### Impact Evidence
- [DHIS2: 30 Years of Health Information Infrastructure](https://dhis2.org/impact/) — Country-level impact across 100+ countries.
- [MOSIP Country Implementations](https://mosip.io/country.php) — National ID deployments across Africa and Asia.
- [Mojaloop Impact Report](https://mojaloop.io/impact/) — Financial inclusion through open payment infrastructure.
- [India Stack Impact](https://indiastack.org/) — 1.3B identities, $2T+ in UPI transactions annually.

### Policy Briefs
- [OECD Going Digital Policy Notes](https://www.oecd.org/going-digital/policy-notes.htm) — Country-specific digital transformation guidance.
- [AfDB Digital Transformation Strategy](https://www.afdb.org/en/topics-and-sectors/topics/digital-transformation) — Africa digital infrastructure priorities.
- [G20 DPI Framework](https://www.g20.org/) — G20 presidency DPI commitments and principles.

---

## Courses & Learning

> Free MOOCs, certifications, and structured learning paths for DPI/DPG practitioners.

### Free Online Courses
| Course | Provider | Level |
|--------|----------|-------|
| [DPI Academy](https://www.undp.org/digital/academy) | UNDP | Beginner–Intermediate |
| [ITU Academy](https://academy.itu.int/) | ITU | All levels |
| [DHIS2 Academy](https://dhis2.org/academy/) | DHIS2 | Beginner–Advanced |
| [GovStack Learning Path](https://www.govstack.global/learning/) | GovStack | Technical |
| [Digital Principles e-Learning](https://digitalprinciples.org/learn/) | DIAL | Beginner |
| [ODK Documentation](https://docs.getodk.org/) | ODK | Technical |

### Certifications
- [ISACA CGEIT](https://www.isaca.org/credentialing/cgeit) — Governance of Enterprise IT (recognized in public sector).
- [Project DPG Certification](https://digitalpublicgoods.net/) — Understanding the DPG standard and certification process.

---

## Jobs & Opportunities

> Where to find roles at the intersection of technology, development, and government.

### Job Boards
| Platform | Focus |
|----------|-------|
| [DevNetJobs](https://www.devnetjobs.org/) | International development tech roles |
| [ReliefWeb Jobs](https://reliefweb.int/jobs) | Humanitarian and development positions |
| [UN Careers](https://careers.un.org/) | UN Secretariat and agency roles |
| [UNICEF Careers](https://www.unicef.org/careers/) | ICT, innovation, and DPG roles |
| [ICTworks Job Board](https://www.ictworks.org/category/jobs/) | ICT for development |
| [LinkedIn #GovTech](https://www.linkedin.com/jobs/) | Search: `DPI`, `DPG`, `GovTech`, `Digital Transformation` |

### Fellowships, Grants & Funding
| Opportunity | Who It's For |
|-------------|--------------|
| [UNICEF Venture Fund](https://www.unicef.org/innovation/venturefund) | DPG startups in low-income countries — equity-free funding |
| [Digital Square Open Calls](https://digitalsquare.org/opencalls) | Grants for global digital health goods |
| [DIAL Fellowship](https://digitalimpactalliance.org/get-involved/) | Digital development practitioners |
| [Co-Develop Country Grants](https://www.co-develop.net/) | Governments implementing DPI |

---

## 🏕️ Field Notes — Real Implementation Insights

> Hard-won lessons from practitioners. Not found in any framework document.
> *Contributed by practitioners with field experience in UNICEF, UNDP, and national government deployments.*

### From the Ground: Timor-Leste & Pacific Island States
Working in fragile states and small island developing states reveals realities no framework covers:

- **📶 Infrastructure before applications:** In fragile states, lightweight tools like KoboToolbox outperform complex HMIS until reliable network and device capacity exist. Don't let "DPI" ambitions outpace infrastructure reality.
- **🤝 Ministry buy-in is the bottleneck:** Technical implementation takes weeks. Stakeholder alignment — across ministries, donors, and civil society — takes months. Budget for this explicitly.
- **🔑 Consistent period identifiers from day one:** Cross-system reporting requires uniform cycle IDs (e.g., `MSSI_2026_q1`) enforced at the data collection layer. Retrofitting later costs 10x more.
- **📄 Design for PDF too:** Even with digital infrastructure, email + PDF remains the de facto channel for senior government officials. Always design for both channels.
- **🌊 Pacific context is unique:** With 14 Pacific island nations spread across millions of km², multi-country DPI requires solutions that work offline, across jurisdictions, and with minimal local tech capacity.

### Common DPI Pitfalls (Anywhere)

| Pitfall | What It Looks Like | How to Avoid |
|--------|-------------------|--------------|
| **Vendor lock-in as DPI** | Proprietary "open" solutions with closed APIs | Verify open APIs, exportable data, no proprietary lock |
| **Digital-first without analog inclusion** | 30-40% of populations lack smartphones | Design for USSD, IVR, and in-person fallback |
| **Sustainability gaps** | Donor-funded projects with no ops budget | Budget for operations from day one, before features |
| **Interoperability as afterthought** | Connecting siloed systems post-launch | Start with integration architecture, not features |
| **Data without governance** | Collecting data without privacy frameworks | Data governance before data collection |
| **Copying India Stack wholesale** | Assuming one country's DPI fits all contexts | Adapt to local legal, political, and capacity context |

---

## Contributing

Contributions are welcome and encouraged! This list grows with input from practitioners, developers, policymakers, and researchers worldwide.

**To add a resource:**
1. Read the [Contribution Guidelines](CONTRIBUTING.md)
2. [Open an issue](../../issues/new/choose) using the **Add Resource** template
3. Or submit a Pull Request directly

**What we're looking for:**
- ✅ Open-source tools with active maintenance
- ✅ Country implementation case studies
- ✅ Field notes and practitioner insights
- ✅ Frameworks from credible international organizations
- ❌ Proprietary commercial solutions
- ❌ Inactive or abandoned projects

---

## License

[![CC0](https://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, the contributors have waived all copyright and related or neighboring rights to this work. See [LICENSE](LICENSE) for details.

---

<div align="center">

**⭐ If this list helped you, please star it and share with your network ⭐**

*Built by practitioners, for practitioners.*

</div>