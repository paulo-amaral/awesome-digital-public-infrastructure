# Awesome Digital Public Infrastructure 

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re) [![Contributions Welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg)](CONTRIBUTING.md) [![Last Updated](https://img.shields.io/github/last-commit/paulo-amaral/awesome-digital-public-infrastructure)](https://github.com/paulo-amaral/awesome-digital-public-infrastructure/commits/main) [![Latest Release](https://img.shields.io/github/v/release/paulo-amaral/awesome-digital-public-infrastructure?label=release)](https://github.com/paulo-amaral/awesome-digital-public-infrastructure/releases)

A list of Digital Public Infrastructure (DPI) and Digital Public Goods (DPG) resources I've found useful — tools, frameworks, country implementations, and things I've learned working in the field.

DPI is the shared digital layer a country builds so that identity, payments, and data exchange work for everyone, not just those with access to private services. DPGs are the open-source software and standards that make this possible without locking governments into proprietary systems.

> Built from field work with UNICEF, UNDP, and government teams across Asia, the Pacific, and fragile states.
> Website: [paulo-amaral.github.io](https://paulo-amaral.github.io/)

---

## Contents

- [💡 Why DPI Matters](#why-dpi-matters)
- [📐 Frameworks & Standards](#frameworks--standards)
- [✅ Certified DPGs by Domain](#certified-dpgs-by-domain)
  - [🏥 Health](#health)
  - [🪪 Identity & Civil Registration](#identity--civil-registration)
  - [💳 Payments & Financial Inclusion](#payments--financial-inclusion)
  - [🎓 Education](#education)
  - [🌿 Climate & Environment](#climate--environment)
  - [🔗 Data Exchange & Interoperability](#data-exchange--interoperability)
  - [🛡️ Child Protection & Social Protection](#child-protection--social-protection)
- [🌍 Country DPI Stacks](#country-dpi-stacks)
- [🧰 Toolkits & Assessment Frameworks](#toolkits--assessment-frameworks)
- [🏛️ Organizations & Communities](#organizations--communities)
- [📚 Research & Reports](#research--reports)
- [🎓 Courses & Learning](#courses--learning)
- [🏕️ Field Notes](#field-notes)
- [🤝 Contributing](#contributing)

---

## 💡 Why DPI Matters

> *"DPI is to the digital economy what roads, electricity, and water are to the physical economy."*
> Co-Develop Fund

Countries with good DPI can deliver services faster, reach more people, and avoid paying license fees to vendors for every new system. Countries without it keep rebuilding the same thing in every ministry.

- India's UPI processes over 10 billion payment transactions per month
- MOSIP gives people a foundational national ID even when they have no other documents
- Shared infrastructure means you build once and reuse across sectors
- The DPG model cuts the cost of digital transformation significantly

As of 2025, over 50 countries are actively building or expanding DPI. The DPG registry lists 140+ certified open-source solutions across health, education, identity, payments, and climate.

---

## 📐 Frameworks & Standards

The main reference points for anyone working on DPI or evaluating DPGs.

### 🏗️ DPI Core Frameworks

- [UNDP Digital Public Goods Standard](https://digitalpublicgoods.net/standard/) — nine criteria a solution must meet to be certified as a DPG
- [DPGA DPGs for DPI Collection](https://www.digitalpublicgoods.net/collections/coll-dpi) — curated set of certified DPGs mapped to the four DPI use cases: identity, payments, data exchange, and government transfers
- [GovStack Reference Architecture](https://specs.govstack.global/) — a building-block model for assembling government digital services
- [ITU Digital Transformation Framework](https://www.itu.int/en/ITU-D/Pages/default.aspx) — guidelines and metrics from the ITU for national digital transformation
- [OECD Digital Government Policy Framework](https://www.oecd.org/governance/digital-government/oecd-digital-government-policy-framework.htm) — six dimensions for assessing how mature a country's digital government is
- [World Bank DPI Framework](https://www.worldbank.org/en/topic/digitaldevelopment) — policy and investment guidance for national digital infrastructure
- [Co-Develop DPI Framework](https://www.co-develop.net/) — practical guidance for countries designing their own DPI
- [Principles for Digital Development](https://digitalprinciples.org/) — nine principles adopted by 300+ organizations working in tech and development
- [DPI Safeguards Framework](https://www.co-develop.net/dpi-safeguards) — rights-based guidance for DPI design
- [IDEA International — DPI & Democracy](https://www.idea.int/theme/digital-public-infrastructure) — how DPI shapes electoral integrity, civic participation, and democratic governance

### 🤖 AI & Emerging Technology

- [OECD AI Principles](https://oecd.ai/en/ai-principles) — the first intergovernmental standard on AI, adopted by 46 countries; covers transparency, accountability, and robustness
- [OECD AI Policy Observatory](https://oecd.ai/) — live database of national AI strategies, policies, and tools from 70+ countries
- [UNESCO Recommendation on the Ethics of AI](https://www.unesco.org/en/artificial-intelligence/recommendation-ethics) — the only global normative framework on AI ethics, adopted by all 193 UNESCO member states
- [UNDP AI for Development](https://www.undp.org/digital/artificial-intelligence) — UNDP's approach to AI in development contexts, including governance and inclusion
- [UNDP Accelerator Labs](https://acceleratorlabs.undp.org/) — network of 91 labs applying AI and frontier tech to development challenges in low-income countries
- [EU AI Act](https://digital-strategy.ec.europa.eu/en/policies/regulatory-framework-ai) — the world's first comprehensive AI regulation, risk-based approach, binding for EU and relevant for any country building AI-based DPI
- [ITU AI for Good](https://aiforgood.itu.int/) — ITU platform connecting AI solutions to UN Sustainable Development Goals
- [G20 AI Principles](https://www.g20.org/) — G20-endorsed principles building on OECD, covering responsible AI across member economies
- [World Bank AI Governance Framework](https://www.worldbank.org/en/topic/digitaldevelopment/brief/ai-in-development) — guidance for low-income countries deploying AI in public services

### 📜 Digital Markets & Regulation

- [EU Digital Markets Act (DMA)](https://digital-markets-act.ec.europa.eu/) — EU regulation targeting gatekeepers in digital markets; relevant model for governments designing open digital infrastructure rules
- [EU Digital Services Act (DSA)](https://digital-strategy.ec.europa.eu/en/policies/digital-services-act-package) — accountability framework for online platforms; complements DPI by setting rules for private layers
- [EU Data Governance Act](https://digital-strategy.ec.europa.eu/en/policies/data-governance-act) — framework for data sharing and data intermediaries; directly relevant to data exchange DPI components
- [EU Data Act](https://digital-strategy.ec.europa.eu/en/policies/data-act) — rules on who can access and use data generated by connected devices and services
- [OECD Going Digital Toolkit](https://goingdigital.oecd.org/) — policy assessment tool covering connectivity, digital government, data, and regulation across 50+ indicators
- [African Union Data Policy Framework](https://au.int/en/documents/20220526/au-data-policy-framework) — AU-level guidance on data governance, cross-border flows, and digital public infrastructure for Africa

### 🌏 Regional Digital Strategies

- [ASEAN Digital Masterplan 2025](https://asean.org/) — regional framework covering digital infrastructure, services, and inclusion across Southeast Asia
- [Pacific Digital Economy Programme (PDEP)](https://www.thepalm.org/) — Pacific Islands digital economy and e-government programs covering 14 nations
- [Smart Africa Blueprint](https://smartafrica.org/) — pan-African digital transformation framework adopted by 38 African heads of state
- [Digital Economy for Africa (DE4A)](https://www.worldbank.org/en/programs/all-africa-digital-transformation) — World Bank initiative to connect every African individual, business, and government digitally by 2030

---

## ✅ Certified DPGs by Domain

Software certified by the [Digital Public Goods Alliance](https://digitalpublicgoods.net/) as open-source and aligned with at least one SDG.

### 🏥 Health

| Solution | What it does | Countries | License |
|----------|-------------|-----------|---------|
| [DHIS2](https://dhis2.org/) | Health data management — the most widely deployed system in the world | 100+ | BSD |
| [OpenMRS](https://openmrs.org/) | Medical records for facilities with limited resources | 40+ | MPL 2.0 |
| [OpenHIM](http://openhim.org/) | Middleware for health data exchange, openHIE reference implementation | — | MPL 2.0 |
| [iHRIS](https://www.ihris.org/) | Health workforce management and planning | 20+ | GPL 3.0 |
| [Bahmni](https://www.bahmni.org/) | Hospital information system built for low-resource settings | 50+ | AGPL 3.0 |
| [OpenELIS](https://openelis-global.org/) | Laboratory information system for public health labs | — | MPL 2.0 |

### 🪪 Identity & Civil Registration

| Solution | What it does | Countries | License |
|----------|-------------|-----------|---------|
| [MOSIP](https://mosip.io/) | Open-source foundational national ID platform | 10+ | MPL 2.0 |
| [OpenCRVS](https://www.opencrvs.org/) | Civil registration — births, deaths, marriages | 10+ | MPL 2.0 |
| [OpenSPP](https://openspp.org/) | Social protection registry built on open standards | — | LGPL 3.0 |
| [OpenG2P](https://openg2p.org/) | Government-to-person benefit delivery | — | MPL 2.0 |
| [QuarkID](https://quarkid.org/) | Decentralized identity using W3C DIDs and Verifiable Credentials | — | Apache 2.0 |
| [DIGIT](https://digit.org/) | Urban governance platform for municipal service delivery | 10+ | MIT |

### 💳 Payments & Financial Inclusion

| Solution | What it does | Countries | License |
|----------|-------------|-----------|---------|
| [Mojaloop](https://mojaloop.io/) | Open payment switch designed for financial inclusion | 10+ | Apache 2.0 |
| [OpenG2P](https://openg2p.org/) | Cash transfers, vouchers, and social benefit payments | — | MPL 2.0 |
| [Mifos X](https://mifos.org/) | Core banking for microfinance institutions | 30+ | MPL 2.0 |
| [Apache Fineract](https://fineract.apache.org/) | Open banking platform for financial services | — | Apache 2.0 |

### 🎓 Education

| Solution | What it does | Users | License |
|----------|-------------|-------|---------|
| [Moodle](https://moodle.org/) | The most widely deployed learning management system | 300M+ | GPL 3.0 |
| [H5P](https://h5p.org/) | Interactive content for online learning | — | MIT |
| [Kolibri](https://learningequality.org/kolibri/) | Works offline, designed for schools with no reliable internet | — | MIT |
| [OpenEDX](https://openedx.org/) | Powers edX and over 100 national deployments | — | AGPL 3.0 |
| [Sunbird](https://sunbird.org/) | India's DIKSHA learning platform, open-sourced | 250M+ | MIT |

### 🌿 Climate & Environment

| Solution | What it does | License |
|----------|-------------|---------|
| [OpenClimate](https://openclimate.network/) | Open data infrastructure for tracking climate action | Apache 2.0 |
| [SEPAL](https://sepal.io/) | FAO platform for forest monitoring and geospatial analysis | MIT |
| [ODK](https://getodk.org/) | Mobile data collection for field monitoring | Apache 2.0 |

### 🔗 Data Exchange & Interoperability

| Solution | What it does | License |
|----------|-------------|---------|
| [X-Road](https://x-road.global/) | Data exchange backbone behind Estonia's entire e-government | MIT |
| [OpenFn](https://www.openfn.org/) | Workflow automation and system interoperability middleware, deployed in 40+ LMICs | LGPL 3.0 |
| [OpenHIE](https://ohie.org/) | Health information exchange architecture and community | — |
| [FHIR (HL7)](https://hl7.org/fhir/) | Global standard for healthcare data exchange | — |
| [KoboToolbox](https://www.kobotoolbox.org/) | Data collection built for humanitarian and development work | GPL |
| [CommCare](https://www.dimagi.com/commcare/) | Mobile data collection for frontline health workers | Apache 2.0 |

### 🛡️ Child Protection & Social Protection

| Solution | What it does | License |
|----------|-------------|---------|
| [Primero](https://www.primero.org/) | Case management for child protection, used by UNICEF, UNHCR, IRC | AGPL 3.0 |
| [RapidPro](https://app.rapidpro.io/) | Messaging platform for humanitarian programs | AGPL 3.0 |
| [CPIMS+](https://www.cpimsglobal.org/) | Child protection information management | AGPL 3.0 |
| [OpenSRP](https://smartregister.org/) | Community health worker register and tracking | Apache 2.0 |

---

## 🌍 Country DPI Stacks

Real country implementations with detailed profiles on what they built, what worked, and what didn't.

| Country | Population | What they built | Profile |
|---------|------------|----------------|---------|
| 🇮🇳 India | 1.4B | Aadhaar, UPI, ONDC, DigiLocker, ABDM | [India](docs/country-profiles/india.md) |
| 🇪🇪 Estonia | 1.4M | X-Road, e-Residency, KSI Blockchain, i-Voting | [Estonia](docs/country-profiles/estonia.md) |
| 🇧🇷 Brazil | 215M | PIX, GOV.BR, Open Finance, Conecte SUS | [Brazil](docs/country-profiles/brazil.md) |
| 🇹🇱 Timor-Leste | 1.3M | CPMIS, e-SISCA, RDTL digital services | [Timor-Leste](docs/country-profiles/timor-leste.md) |
| 🇰🇪 Kenya | 55M | Huduma Namba, M-Pesa, eCitizen | coming soon |
| 🇷🇼 Rwanda | 14M | Irembo, National ID, mobile money | coming soon |
| 🇵🇭 Philippines | 115M | PhilSys, InstaPay, eGovPH | coming soon |
| 🇸🇳 Senegal | 17M | Wari, Orange Money, DER programs | coming soon |
| 🇫🇯 Fiji | 900K | Digital Fiji strategy, mHealth pilots | coming soon |

Want to contribute a country profile? See [CONTRIBUTING.md](CONTRIBUTING.md).

---

## 🧰 Toolkits & Assessment Frameworks

### 📊 Digital Readiness & Assessment

- [ITU ICT Development Index](https://www.itu.int/en/ITU-D/Statistics/Pages/publications/mis/methodology.aspx) — benchmarks digital readiness across 167 countries
- [OECD Digital Government Index](https://www.oecd.org/governance/digital-government/digital-government-index.htm) — maturity model covering six dimensions of digital government
- [DIAL Digital Investment Framework](https://dial.global/) — helps prioritize DPG investments
- [WEF Global Technology Governance Report](https://www.weforum.org/reports/global-technology-governance-report-2021/) — framework for responsible DPI deployment
- [GovStack Digital Readiness Assessment](https://www.govstack.global/) — country readiness tool for building-block-based DPI

### 🔌 Interoperability

- [GovStack Building Blocks Specification](https://govstack.gitbook.io/specification/) — technical specs for interoperable government services
- [OpenHIE Architecture](https://ohie.org/framework/) — health information exchange reference architecture
- [IHE Integration Profiles](https://www.ihe.net/resources/profiles/) — integration profiles for healthcare interoperability

### 📋 Procurement & Policy

- [UNICEF Venture Fund Guidance](https://www.unicef.org/innovation/venturefund) — how to fund and scale DPGs in low-income countries
- [Digital Square Global Goods Maturity Model](https://digitalsquare.org/global-goods-maturity-model) — maturity model for health digital tools
- [Open Source Policy Guide](https://github.com/todogroup/ospology) — policy frameworks and OSPO guidance for government open-source adoption
- [ITU Model Policy on Open Source](https://www.itu.int/) — ITU guidance for national open-source policies

---

## 🏛️ Organizations & Communities

### 🌐 UN System & Multilaterals

| Organization | What they do |
|---|---|
| [Digital Public Goods Alliance (DPGA)](https://digitalpublicgoods.net/) | Defines and certifies DPGs |
| [UNICEF Office of Innovation](https://www.unicef.org/innovation/) | Funds DPGs and frontier tech for children |
| [UNDP Digital](https://www.undp.org/digital) | Digital transformation in 170+ countries |
| [ITU](https://www.itu.int/) | UN agency for ICTs |
| [World Bank Digital Development](https://www.worldbank.org/en/topic/digitaldevelopment) | Finances digital infrastructure |
| [UN OICT](https://unite.un.org/) | UN Office of ICT |

### 🤲 Foundations & Alliances

| Organization | Focus |
|---|---|
| [Digital Impact Alliance (DIAL)](https://digitalimpactalliance.org/) | Research on digital development |
| [Digital Square](https://digitalsquare.org/) | Grants for global digital health tools |
| [Co-Develop Fund](https://www.co-develop.net/) | Philanthropic funding for DPI in low-income countries |
| [Gates Foundation](https://www.gatesfoundation.org/our-work/programs/global-growth-and-opportunity/inclusive-financial-systems) | Financial inclusion |
| [Omidyar Network](https://omidyar.com/) | Investment in DPI and open internet |
| [Rockefeller Foundation](https://www.rockefellerfoundation.org/) | Digital equity |

### 💻 Technical Communities

- [GovStack Community](https://www.govstack.global/) — people building reusable government building blocks
- [OpenHIE Community](https://ohie.org/) — health information exchange implementers worldwide
- [Digital Development Forum](https://www.digitaldevelopment.org/) — ICT4D community of practice
- [ICTworks](https://www.ictworks.org/) — good resource hub for digital development professionals

---

## 📚 Research & Reports

### 📖 Start Here

- [DPI-AI Framework: Building AI-Ready Nations through Digital Public Infrastructure](https://digitalpublicinfrastructure.ai/) — CDPI vision paper (2026) on embedding AI into DPI via AI Blocks, DPI Workflows, and Public Agents; CC BY 4.0
- [The Agentic State: Rethinking Government for the Era of Agentic AI](https://agenticstate.org/) — vision paper (2025, Global GovTech Centre / World Bank) covering AI in public services, workflows, procurement, governance, and crisis response; launched at Tallinn Digital Summit
- [Digital Public Infrastructure and Development: A World Bank Group Approach](https://documents1.worldbank.org/curated/en/099031025172027713/pdf/P505739-84c5073b-9d40-4b83-a211-98b2263e87dd.pdf) — World Bank Digital Transformation White Paper, Vol. 1 (2025)
- [The Case for a New Digital Bretton Woods](https://www.bu.edu/gdp/) — Boston University Global Development Policy Center
- [The Economics of Digital Public Infrastructure](https://dial.global/research/economics-of-digital-public-infrastructure/) — DIAL / Co-Develop research on DPI's economic case for equitable growth
- [Rethinking Digital Public Infrastructure](https://www3.weforum.org/docs/WEF_Rethinking_Digital_Public_Infrastructure.pdf) — World Economic Forum
- [Digital Public Infrastructure and Democracy](https://omidyarnetwork.com/) — Omidyar Network

### 📈 Impact Evidence

- [DHIS2: 30 Years of Health Information Infrastructure](https://dhis2.org/impact/) — country-level impact across 100+ countries
- [MOSIP Country Implementations](https://mosip.io/country.php) — national ID deployments across Africa and Asia
- [Mojaloop Impact Report](https://mojaloop.io/) — financial inclusion through open payments
- [India Stack Impact](https://indiastack.org/) — 1.3B identities, $2T+ in UPI transactions annually

### 📜 Policy

- [OECD Going Digital Policy Notes](https://www.oecd.org/going-digital/policy-notes.htm) — country-specific digital transformation guidance
- [AfDB Digital Transformation Strategy](https://www.afdb.org/en/topics-and-sectors/topics/digital-transformation) — Africa's digital infrastructure priorities
- [G20 DPI Framework](https://www.g20.org/) — G20 DPI commitments and principles

### 👩‍💻 Digital Workforce & Inclusion

- [Where is Digital Youth Work? Policy Invisibility and the Case for Recognition](https://dywrhubreport2026.netlify.app/) — University of Leeds / INCLUDE+ Network (2026); reviews 800+ government bodies and 26 policies to show how youth workers — the most effective digital inclusion practitioners — are systematically excluded from policy and funding

---

## 🎓 Courses & Learning

### 🖥️ Free Courses

| Course | Provider | Level |
|--------|----------|-------|
| [DPI Academy](https://www.undp.org/digital/academy) | UNDP | Beginner to Intermediate |
| [ITU Academy](https://academy.itu.int/) | ITU | All levels |
| [DHIS2 Academy](https://dhis2.org/academy/) | DHIS2 | Beginner to Advanced |
| [GovStack Learning Path](https://govstack.global/) | GovStack | Technical |
| [Digital Principles e-Learning](https://digitalprinciples.org/principles/) | DIAL | Beginner |
| [ODK Documentation](https://docs.getodk.org/) | ODK | Technical |

### 🏅 Certifications

- [ISACA CGEIT](https://www.isaca.org/credentialing/cgeit) — governance of enterprise IT, recognized in the public sector
- [Project DPG Certification](https://digitalpublicgoods.net/) — understanding the DPG standard and certification process

---

## 🏕️ Field Notes

Things learned working in the field that don't appear in any framework document. Built from implementations with UNICEF, UNDP, and government teams across Timor-Leste, the Pacific, and fragile states.

| Note | Topics |
|------|--------|
| [🌴 Timor-Leste and the Pacific](docs/field-notes/timor-leste-pacific.md) | Fragile states, ministry alignment, identifiers, offline tools |
| [🧑‍🤝‍🧑 Design & Architecture](docs/field-notes/design-architecture.md) | HCD, service blueprints, user journeys, TOGAF |
| [📵 Offline-First & Last Mile](docs/field-notes/offline-first.md) | Connectivity, sync, device testing, 2G |
| [⚖️ Digital Divide, AI Divide & Inclusion](docs/field-notes/digital-divide-inclusion.md) | Gender, disability, language, AI divide |
| [🌐 Emerging Technologies](docs/field-notes/emerging-technologies.md) | Drones, AgriTech, AI, data readiness |
| [🏛️ Policies, Standards & Laws](docs/field-notes/policies-standards-laws.md) | Legal alignment, data protection, standards, governance |
| [⚠️ Common Mistakes](docs/field-notes/common-mistakes.md) | Vendor lock-in, sustainability, interoperability |

→ [Browse all field notes](docs/field-notes/README.md)

---

## 🤝 Contributing

This list is kept up to date with contributions from people working in government, international organizations, and open-source development. If you know something that should be here, add it.

**How to add a resource:**
1. Read [CONTRIBUTING.md](CONTRIBUTING.md)
2. [Open an issue](https://github.com/paulo-amaral/awesome-digital-public-infrastructure/issues/new/choose) using the Add Resource template
3. Or submit a pull request directly

**What belongs here:**
- Open-source tools with active maintenance
- Country implementation case studies
- Field notes from real deployments
- Frameworks from recognized international organizations

**What doesn't:**
- Proprietary tools, even with a free tier
- Inactive or abandoned projects

---

## License

<div align="center">

[<img src="https://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg" alt="CC0 1.0 Public Domain" height="36">](https://creativecommons.org/publicdomain/zero/1.0/)
&nbsp;&nbsp;
[<img src="https://mirrors.creativecommons.org/presskit/logos/cc.logo.svg" alt="Creative Commons" height="36">](https://creativecommons.org/)
&nbsp;&nbsp;
[<img src="https://img.shields.io/badge/Open%20Source-Initiative-3DA639?style=for-the-badge&logo=opensourceinitiative&logoColor=white" alt="Open Source Initiative" height="36">](https://opensource.org/)

<sub>Content is CC0 — public domain. All software listed is open source. See each project's license for details.</sub>

</div>

---

<div align="center">

If this list was useful, star it and pass it on.

[paulo-amaral.github.io](https://paulo-amaral.github.io/)

*Made with ❤️ in the 🐊 island*

</div>
