# Awesome Digital Public Infrastructure

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re) [![Contributions Welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg)](CONTRIBUTING.md) [![Last Updated](https://img.shields.io/github/last-commit/paulo-amaral/awesome-digital-public-infrastructure)](https://github.com/paulo-amaral/awesome-digital-public-infrastructure/commits/main) [![Latest Release](https://img.shields.io/github/v/release/paulo-amaral/awesome-digital-public-infrastructure?label=release)](https://github.com/paulo-amaral/awesome-digital-public-infrastructure/releases)

A list of Digital Public Infrastructure (DPI) and Digital Public Goods (DPG) resources I've found useful - tools, frameworks, country implementations, and things I've learned working in the field.

DPI is the shared digital layer a country builds so that identity, payments, and data exchange work for everyone, not just those with access to private services. DPGs are the open-source software and standards that make this possible without locking governments into proprietary systems.

> Built from field work with UNICEF, UNDP, and government teams across Asia, the Pacific, and fragile states.
> Website: [paulo-amaral.github.io](https://paulo-amaral.github.io/)

---

## Contents

- [Why DPI Matters](#why-dpi-matters)
- [Frameworks & Standards](#frameworks--standards)
- [Certified DPGs by Domain](#certified-dpgs-by-domain)
  - [Health](#health)
  - [Identity & Civil Registration](#identity--civil-registration)
  - [Payments & Financial Inclusion](#payments--financial-inclusion)
  - [Education](#education)
  - [Civic Participation & Democratic Governance](#civic-participation--democratic-governance)
  - [Climate & Environment](#climate--environment)
  - [Data Exchange & Interoperability](#data-exchange--interoperability)
  - [Child Protection & Social Protection](#child-protection--social-protection)
- [Country DPI Stacks](#country-dpi-stacks)
  - [Regional & Cross-Border DPI](#regional--cross-border-dpi)
- [Toolkits & Assessment Frameworks](#toolkits--assessment-frameworks)
- [Organizations & Communities](#organizations--communities)
- [Research & Reports](#research--reports)
- [Courses & Learning](#courses--learning)
- [Field Notes](#field-notes)
- [Contributing](#contributing)

---

## Why DPI Matters

> *"DPI is to the digital economy what roads, electricity, and water are to the physical economy."*
> Co-Develop Fund

Countries with good DPI can deliver services faster, reach more people, and avoid paying license fees to vendors for every new system. Countries without it keep rebuilding the same thing in every ministry.

- India's UPI processes over 10 billion payment transactions per month
- MOSIP gives people a foundational national ID even when they have no other documents
- Shared infrastructure means you build once and reuse across sectors
- The DPG model cuts the cost of digital transformation significantly

As of 2025, over 50 countries are actively building or expanding DPI. The DPG registry lists 140+ certified open-source solutions across health, education, identity, payments, and climate.

---

## Frameworks & Standards

The main reference points for anyone working on DPI or evaluating DPGs.

### DPI Core Frameworks

- [DPGA Digital Public Goods Standard](https://digitalpublicgoods.net/standard/) - nine criteria a solution must meet to be certified as a DPG
- [DPGA DPGs for DPI Collection](https://www.digitalpublicgoods.net/collections/coll-dpi) - curated set of certified DPGs mapped to the four DPI use cases: identity, payments, data exchange, and government transfers
- [CDPI DPI Wiki](https://docs.cdpi.dev/the-dpi-wiki/dpi-overview) - practical explainer on DPI concepts, architecture principles, and first-use-case selection
- [Global Digital Compact](https://www.un.org/global-digital-compact/en) - UN framework adopted in 2024 that calls for investment in digital public goods and safe, inclusive digital public infrastructure
- [GovStack Reference Architecture](https://specs.govstack.global/) - a building-block model for assembling government digital services
- [GovStack Implementation Playbook](https://specs.govstack.global/implementation-playbook) - step-by-step guide for governments planning, designing, developing, and implementing digital public services
- [GovStack Building Block Software](https://govstack.global/software/) - marketplace/catalogue of software implementing GovStack Building Blocks, with compliance information across deployment, API standards, and requirement specifications
- [ITU Digital Transformation Framework](https://www.itu.int/en/ITU-D/Pages/default.aspx) - guidelines and metrics from the ITU for national digital transformation
- [OECD Digital Government Policy Framework](https://www.oecd.org/governance/digital-government/oecd-digital-government-policy-framework.htm) - six dimensions for assessing how mature a country's digital government is
- [World Bank DPI Framework](https://www.worldbank.org/en/topic/digitaldevelopment) - policy and investment guidance for national digital infrastructure
- [Co-Develop DPI Framework](https://www.codevelop.fund/) - practical guidance for countries designing their own DPI
- [Principles for Digital Development](https://digitalprinciples.org/) - nine principles adopted by 300+ organizations working in tech and development
- [DPI Safeguards Framework](https://www.dpi-safeguards.org/) - rights-based guidance for DPI design
- [IDEA International - DPI & Democracy](https://www.idea.int/theme/digital-public-infrastructure) - how DPI shapes electoral integrity, civic participation, and democratic governance
- [UNDP Digital Public Infrastructure](https://www.undp.org/digital/digital-public-infrastructure) - UNDP's DPI hub covering offerings, safeguards, open source, partners, and country support

### Technical & Security Standards

Where to find the core technical standards behind DPI and how each one maps to a national stack. For a worked example, the [X-Road Simulator compliance matrix](https://github.com/paulo-amaral/xroad-simulator/blob/main/docs/technical-standards-compliance.md) maps every norm below to a running data-exchange sandbox, with met/partial/gap status.

- [ISO/IEC 27001 & 27002](https://www.iso.org/standard/27001) - information security management (ISMS); the baseline for any agency operating identity, payments, or data exchange as critical infrastructure
- [ISO/IEC 27701](https://www.iso.org/standard/71670.html) - privacy information management extension of 27001; operationalizes data protection laws for DPI operators
- [NIST SP 800-63-4 Digital Identity Guidelines](https://pages.nist.gov/800-63-4/) - identity and authenticator assurance levels (IAL/AAL) that national digital ID programs use to calibrate onboarding and login risk
- [NIST Cybersecurity Framework 2.0](https://www.nist.gov/cyberframework) - govern, identify, protect, detect, respond, recover; the common language between DPI operators and national CERTs
- [NIST FIPS 140-3](https://csrc.nist.gov/pubs/fips/140-3/final) - cryptographic module (HSM) validation for the keys behind national CAs and digital signatures
- [ETSI EN 319 series / eIDAS](https://www.etsi.org/technologies/electronic-signature) - PAdES, XAdES, and CAdES legally valid electronic signatures; the trust framework that X-Road message signing aligns with
- [W3C Verifiable Credentials](https://www.w3.org/TR/vc-data-model-2.0/) - data model behind wallet-based credentials and document verification services such as verify.gov.kh
- [W3C WCAG 2.2](https://www.w3.org/TR/WCAG22/) - level AA as the accessibility floor for citizen-facing services
- [IETF RFC Editor](https://www.rfc-editor.org/) - the plumbing of secure data exchange: TLS 1.3 (RFC 8446), X.509 PKI (RFC 5280), OCSP (RFC 6960), time-stamping (RFC 3161), OAuth 2.0 and PKCE (RFC 6749, 7636), JWT best practices (RFC 8725)
- [OpenID Connect](https://openid.net/specs/openid-connect-core-1_0.html) - citizen single sign-on and consented authorization for government portals
- [OpenAPI 3.1](https://spec.openapis.org/oas/latest.html) - API contracts for every service published on a data exchange layer
- [OWASP ASVS](https://owasp.org/www-project-application-security-verification-standard/) - application security verification (level 2 minimum) for public-facing services
- [Open Contracting Data Standard](https://standard.open-contracting.org/) - open procurement data; with SBOM and source escrow clauses it is the anti lock-in toolkit for DPI contracts

### DPI & DPG Approaches

Different organizations use complementary lenses for DPI and DPGs: architecture, safeguards, open-source reuse, country roadmaps, rapid deployment, and sector-specific stacks.

- [CDPI DPG and DPI](https://docs.cdpi.dev/the-dpi-wiki/dpg-and-dpi) - explains the relationship between digital public goods as reusable open-source products and digital public infrastructure as country-scale systems
- [CDPI DPI Architecture Principles](https://docs.cdpi.dev/the-dpi-wiki/dpi-tech-architecture-principles) - five technical principles for DPI: interoperability, minimalist reusable building blocks, ecosystem innovation, federation/decentralization, and security/privacy by design
- [CDPI DaaS Way](https://cdpi.dev/daas/) - rapid DPI deployment approach using open-source DPGs, pre-qualified service providers, and ready-to-deploy program, policy, legal, and technical artefacts
- [CDPI DPI-AI Framework](https://digitalpublicinfrastructure.ai/) - 2026 framework for AI-ready public services using AI Blocks, DPI Workflows, and Public Agents on top of existing DPI foundations
- [DPGA DPGs for DPI Approach](https://www.digitalpublicgoods.net/collections/coll-dpi) - maps certified digital public goods to DPI use cases such as identity, payments, data exchange, and government transfers
- [GovStack Building Block Approach](https://specs.govstack.global/) - modular architecture approach for assembling reusable, interoperable government digital service capabilities
- [UNDP DPI Approach Playbook](https://www.undp.org/sites/g/files/zskgke326/files/2023-08/undp-the-dpi-approach-a-playbook.pdf) - direct PDF playbook for country teams, with six practical plays covering DPI scoping, technology, governance, sustainability, and implementation
- [UN 2.0 entry: The Digital Public Infrastructure Approach](https://un-two-zero.network/contents/the-digital-public-infrastructure-approach-a-playbook/) - UN catalogue page for the UNDP playbook, positioning it as a practical public resource for low- and middle-income countries building inclusive, rights-based DPI
- [Universal DPI Safeguards Approach](https://www.dpi-safeguards.org/framework) - rights-based approach focused on accountability, inclusion, privacy, safety, and participatory governance across the DPI lifecycle
- [World Bank Global DPI Program](https://www.worldbank.org/en/results/2026/05/06/global-digital-public-infrastructure-program) - cross-sector country programme approach centered on digital ID, payments, and secure data sharing across 80+ countries

### AI & Emerging Technology

- [OECD AI Principles](https://oecd.ai/en/ai-principles) - the first intergovernmental standard on AI, adopted by 46 countries; covers transparency, accountability, and robustness
- [OECD AI Policy Observatory](https://oecd.ai/) - live database of national AI strategies, policies, and tools from 70+ countries
- [UNESCO Recommendation on the Ethics of AI](https://www.unesco.org/en/artificial-intelligence/recommendation-ethics) - the only global normative framework on AI ethics, adopted by all 193 UNESCO member states
- [UNDP AI for Development](https://www.undp.org/digital/artificial-intelligence) - UNDP's approach to AI in development contexts, including governance and inclusion
- [UNDP Accelerator Labs](https://acceleratorlabs.undp.org/) - network of 91 labs applying AI and frontier tech to development challenges in low-income countries
- [EU AI Act](https://digital-strategy.ec.europa.eu/en/policies/regulatory-framework-ai) - the world's first comprehensive AI regulation, risk-based approach, binding for EU and relevant for any country building AI-based DPI
- [ITU AI for Good](https://aiforgood.itu.int/) - ITU platform connecting AI solutions to UN Sustainable Development Goals
- [G20 AI Principles](https://www.g20.org/) - G20-endorsed principles building on OECD, covering responsible AI across member economies
- [World Bank AI Governance Framework](https://www.worldbank.org/en/topic/digitaldevelopment/brief/ai-in-development) - guidance for low-income countries deploying AI in public services

### Digital Markets & Regulation

- [EU Digital Markets Act (DMA)](https://digital-markets-act.ec.europa.eu/) - EU regulation targeting gatekeepers in digital markets; relevant model for governments designing open digital infrastructure rules
- [EU Digital Services Act (DSA)](https://digital-strategy.ec.europa.eu/en/policies/digital-services-act-package) - accountability framework for online platforms; complements DPI by setting rules for private layers
- [EU Data Governance Act](https://digital-strategy.ec.europa.eu/en/policies/data-governance-act) - framework for data sharing and data intermediaries; directly relevant to data exchange DPI components
- [EU Data Act](https://digital-strategy.ec.europa.eu/en/policies/data-act) - rules on who can access and use data generated by connected devices and services
- [OECD Going Digital Toolkit](https://goingdigital.oecd.org/) - policy assessment tool covering connectivity, digital government, data, and regulation across 50+ indicators
- [African Union Data Policy Framework](https://au.int/en/documents/20220526/au-data-policy-framework) - AU-level guidance on data governance, cross-border flows, and digital public infrastructure for Africa

### Regional Digital Strategies

- [ASEAN Digital Masterplan 2025](https://asean.org/) - regional framework covering digital infrastructure, services, and inclusion across Southeast Asia
- [Pacific Digital Economy Programme (PDEP)](https://www.thepalm.org/) - Pacific Islands digital economy and e-government programs covering 14 nations
- [Smart Africa Blueprint](https://smartafrica.org/) - pan-African digital transformation framework adopted by 38 African heads of state
- [Digital Economy for Africa (DE4A)](https://www.worldbank.org/en/programs/all-africa-digital-transformation) - World Bank initiative to connect every African individual, business, and government digitally by 2030
- [Red GEALC](https://www.oas.org/ext/en/democracy/red-gealc) - Latin America and Caribbean digital government cooperation network coordinating regional standards, shared work groups, and cross-border digital government initiatives such as IdLAC

### Legal Informatics & Legislative XML

Standards and frameworks for making legal and legislative documents machine-readable - the infrastructure layer underneath open law data, digital compliance, and e-justice systems.

- [Akoma Ntoso (OASIS LegalDocML v1.0)](https://www.oasis-open.org/standard/akn-v1-0/) - open XML standard (adopted 2018) defining the structure and semantics of parliamentary, legislative, and judicial documents; the name means "linked hearts" in Akan; adopted by the United Nations as the primary format for machine-processable UN documents; used by the UK National Archives, US Congress (USLM), Brazil (LexML), and many parliaments
- [OASIS LegalDocML Technical Committee](https://www.oasis-open.org/committees/tc_home.php?wg_abbrev=legaldocml) - OASIS TC that governs the Akoma Ntoso standard; the international body where governments, parliaments, and researchers converge on interoperable legal document markup
- [LegalRuleML (OASIS)](https://www.oasis-open.org/committees/tc_home.php?wg_abbrev=legalruleml) - companion OASIS standard for the logical-formal representation of legal norms as machine-readable rules; enables automated compliance checking and temporal legal reasoning (what the law said at a given point in time)
- [CIRSFID / LEDS4XAIL - University of Bologna](https://site.unibo.it/leds4xail/en/) - leading interdisciplinary research centre in legal informatics and explainable AI; home of Akoma Ntoso's co-author [Monica Palmirani](https://www.unibo.it/sitoweb/monica.palmirani/pubblicazioni), Full Professor of Legal Informatics and co-chair of the OASIS LegalDocML and LegalRuleML TCs; research spans five areas directly relevant to DPI:
  - **eLegislation** - XML meta-modeling of legal text; dynamic management of norms over time (point-in-time consolidation)
  - **Legal reasoning** - LegalRuleML-based formal models for compliance checking; temporal legal logic
  - **Legal knowledge representation** - ontological modeling of legal knowledge; NLP extraction from legal corpora
  - **eGovernance / eJustice** - digital transformation of public administration, eParticipation, and justice system digitization
  - **Digital rights** - digital identity, privacy, and awareness of fundamental rights in digital environments
- [Lexdatafication](https://cris.unibo.it/handle/11585/843063) - University of Bologna project modelling Italy's complete legal knowledge base in Akoma Ntoso, in cooperation with IPZS (Italy's Official Gazette entity); a blueprint for national-scale open law data built from legacy normative databases
- [Summer School Legislative XML - University of Bologna](http://summerschoollex.cirsfid.unibo.it/) - annual intensive program training public officials and legal technologists on Akoma Ntoso and Legal XML; run by CIRSFID since the early 2000s

---

## Certified DPGs by Domain

Software certified by the [Digital Public Goods Alliance](https://digitalpublicgoods.net/) as open-source and aligned with at least one SDG.

### Health

| Solution | What it does | Countries | License |
|----------|-------------|-----------|---------|
| [DHIS2](https://dhis2.org/) | Health data management - the most widely deployed system in the world | 100+ | BSD |
| [OpenMRS](https://openmrs.org/) | Medical records for facilities with limited resources | 40+ | MPL 2.0 |
| [OpenHIM](http://openhim.org/) | Middleware for health data exchange, openHIE reference implementation | - | MPL 2.0 |
| [iHRIS](https://www.ihris.org/) | Health workforce management and planning | 20+ | GPL 3.0 |
| [Bahmni](https://www.bahmni.org/) | Hospital information system built for low-resource settings | 50+ | AGPL 3.0 |
| [OpenELIS](https://openelis-global.org/) | Laboratory information system for public health labs | - | MPL 2.0 |

### Identity & Civil Registration

| Solution | What it does | Countries | License |
|----------|-------------|-----------|---------|
| [MOSIP](https://mosip.io/) | Open-source foundational national ID platform | 10+ | MPL 2.0 |
| [OpenCRVS](https://www.opencrvs.org/) | Civil registration - births, deaths, marriages | 10+ | MPL 2.0 |
| [OpenSPP](https://openspp.org/) | Social protection registry built on open standards | - | LGPL 3.0 |
| [OpenG2P](https://openg2p.org/) | Government-to-person benefit delivery | - | MPL 2.0 |
| [QuarkID](https://quarkid.org/) | Decentralized identity using W3C DIDs and Verifiable Credentials | - | Apache 2.0 |
| [DIGIT](https://digit.org/) | Urban governance platform for municipal service delivery | 10+ | MIT |

### Payments & Financial Inclusion

| Solution | What it does | Countries | License |
|----------|-------------|-----------|---------|
| [Mojaloop](https://mojaloop.io/) | Open payment switch designed for financial inclusion | 10+ | Apache 2.0 |
| [OpenG2P](https://openg2p.org/) | Cash transfers, vouchers, and social benefit payments | - | MPL 2.0 |
| [Mifos X](https://mifos.org/) | Core banking for microfinance institutions | 30+ | MPL 2.0 |
| [Apache Fineract](https://fineract.apache.org/) | Open banking platform for financial services | - | Apache 2.0 |

### Education

| Solution | What it does | Users | License |
|----------|-------------|-------|---------|
| [Moodle](https://moodle.org/) | The most widely deployed learning management system | 300M+ | GPL 3.0 |
| [H5P](https://h5p.org/) | Interactive content for online learning | - | MIT |
| [Kolibri](https://learningequality.org/kolibri/) | Works offline, designed for schools with no reliable internet | - | MIT |
| [OpenEDX](https://openedx.org/) | Powers edX and over 100 national deployments | - | AGPL 3.0 |
| [Sunbird](https://sunbird.org/) | India's DIKSHA learning platform, open-sourced | 250M+ | MIT |
| [Learning Passport](https://www.learningpassport.org/) | UNICEF online/offline/mobile learning platform for children in crisis and low-connectivity contexts | 10M+ | - |

### Civic Participation & Democratic Governance

| Solution | What it does | Scale | License |
|----------|-------------|-------|---------|
| [Decidim](https://decidim.org/) | Citizen participation platform for participatory democracy, consultations, assemblies, budgeting, and civic collaboration | 30+ countries, 400+ administrations, 50+ NGOs | AGPL 3.0 |

### Climate & Environment

| Solution | What it does | License |
|----------|-------------|---------|
| [OpenClimate](https://openclimate.network/) | Open data infrastructure for tracking climate action | Apache 2.0 |
| [SEPAL](https://sepal.io/) | FAO platform for forest monitoring and geospatial analysis | MIT |
| [ODK](https://getodk.org/) | Mobile data collection for field monitoring | Apache 2.0 |

### Data Exchange & Interoperability

| Solution | What it does | License |
|----------|-------------|---------|
| [X-Road](https://x-road.global/) | Data exchange backbone behind Estonia's entire e-government | MIT |
| [OpenFn](https://www.openfn.org/) | Workflow automation and system interoperability middleware, deployed in 40+ LMICs | LGPL 3.0 |
| [OpenHIE](https://ohie.org/) | Health information exchange architecture and community | - |
| [FHIR (HL7)](https://hl7.org/fhir/) | Global standard for healthcare data exchange | - |
| [KoboToolbox](https://www.kobotoolbox.org/) | Data collection built for humanitarian and development work | GPL |
| [CommCare](https://www.dimagi.com/commcare/) | Mobile data collection for frontline health workers | Apache 2.0 |

### Child Protection & Social Protection

| Solution | What it does | License |
|----------|-------------|---------|
| [Primero](https://www.primero.org/) | Case management for child protection, used by UNICEF, UNHCR, IRC | AGPL 3.0 |
| [RapidPro](https://app.rapidpro.io/) | Messaging platform for humanitarian programs | AGPL 3.0 |
| [CPIMS+](https://www.cpimsglobal.org/) | Child protection information management | AGPL 3.0 |
| [OpenSRP](https://smartregister.org/) | Community health worker register and tracking | Apache 2.0 |

---

## Country DPI Stacks

Real country implementations with detailed profiles on what they built, what worked, and what didn't.

>  **[Explore the DPI Map](https://dpimap.org/)** - UCL IIPP interactive map tracking national DPI across 190+ countries: 68 with Digital ID, 99 with Digital Payments, 103 with Data Exchange systems.

| Country | Population | What they built | Profile |
|---------|------------|----------------|---------|
| India | 1.4B | Aadhaar, UPI, ONDC, DigiLocker, ABDM | [India](docs/country-profiles/india.md) |
| Estonia | 1.4M | X-Road, e-Residency, KSI Blockchain, i-Voting | [Estonia](docs/country-profiles/estonia.md) |
| Brazil | 215M | PIX, GOV.BR, Open Finance, Conecte SUS | [Brazil](docs/country-profiles/brazil.md) |
| Timor-Leste | 1.3M | CPMIS, e-SISCA, RDTL digital services | [Timor-Leste](docs/country-profiles/timor-leste.md) |
| Cambodia | 17M | [CamDX](https://camdx.gov.kh/) (data exchange, X-Road based), [CamDigiKey](https://camdx.gov.kh/docs/open-api/ekyc) (digital ID & e-KYC), [Bakong](https://bakong.nbc.gov.kh/) (blockchain payments), [verify.gov.kh](https://verify.gov.kh/) (document verification; Gold ASEAN Digital Awards 2024, UN Public Service Award 2026, launched in Timor-Leste, rollouts in Laos & Philippines) | [Cambodia](docs/country-profiles/cambodia.md) |
| Kenya | 55M | Huduma Namba, M-Pesa, eCitizen | coming soon |
| Rwanda | 14M | Irembo, National ID, mobile money | coming soon |
| Philippines | 115M | PhilSys, InstaPay, eGovPH | coming soon |
| Senegal | 17M | Wari, Orange Money, DER programs | coming soon |
| Trinidad & Tobago | 1.4M | First DaaS implementation - verifiable credentials at national scale (2025) | coming soon |
| Fiji | 900K | Digital Fiji strategy, mHealth pilots | coming soon |
| Mozambique | 34M | Early-stage talks: [X-Road](https://x-road.global/)-based data exchange with single-window services (balcão único), exploring Ethiopia's [Fayda](https://id.gov.et/) eKYC model (MOSIP-based) | coming soon |

### Regional & Cross-Border DPI

Regional DPI examples where countries agree on shared standards, trust frameworks, and reusable open-source components so citizens and businesses can use national digital credentials across borders.

| Initiative | Region | What it enables | Partners |
|------------|--------|-----------------|----------|
| [IdLAC](https://redgealc.org/idlac/en/home/) | Latin America and the Caribbean | Open-source regional digital identity broker for mutual recognition of national eIDs; supports cross-border access to public services, including Brazil-Uruguay digital service access through national eID credentials | Red GEALC, IDB, World Bank, Co-Develop, OAS |

Participating countries include Argentina, Bolivia, Brazil, Chile, Colombia, Costa Rica, Dominican Republic, Ecuador, Guatemala, Paraguay, Peru, and Uruguay.

Want to contribute a country profile? See [CONTRIBUTING.md](CONTRIBUTING.md).

---

## Toolkits & Assessment Frameworks

### Digital Readiness & Assessment

- [ITU ICT Development Index](https://www.itu.int/en/ITU-D/Statistics/Pages/publications/mis/methodology.aspx) - benchmarks digital readiness across 167 countries
- [OECD Digital Government Index](https://www.oecd.org/governance/digital-government/digital-government-index.htm) - maturity model covering six dimensions of digital government
- [DIAL Digital Investment Framework](https://dial.global/) - helps prioritize DPG investments
- [DPI Roadmap Playbook](https://www.africanenda.org/en/publications/dpi-roadmap-playbook-2) - 2026 country roadmap guide from DIAL, AfricaNenda, Better Than Cash Alliance, and CDPI for planning national DPI priorities
- [WEF Global Technology Governance Report](https://www.weforum.org/reports/global-technology-governance-report-2021/) - framework for responsible DPI deployment
- [GovStack Digital Readiness Assessment](https://www.govstack.global/) - country readiness tool for building-block-based DPI
- [UNDP AILA - AI Landscape Assessment](https://www.undp.org/digital/aila) - national AI readiness framework assessing government, private sector, civil society, and academia; deployed in 15+ countries since 2024
- [UNDP Digital Guides](https://digitalguides.undp.org/) - thematic guides for applying digital transformation to poverty, governance, resilience, environment, energy, and gender
- [UNDP DRA - Digital Readiness Assessment](https://www.undp.org/digital/dra) - cross-cutting hybrid assessment covering five digital transformation pillars; deployed in 50+ countries
- [UNDP Digital Development Compass](https://digitaldevelopmentcompass.undp.org/) - aggregates digital indicators from 140+ open datasets including DPI sub-dimensions: identity, payments, data exchange
- [UNDP Digital Standards](https://www.undp.org/digital/standards) - public digital standards for teams designing and delivering inclusive digital solutions
- [UNDP Governance Assessment Framework for Data Exchange Systems](https://governance4dataexchange.org/) - assessment framework for safe, inclusive, and accountable governance of national data exchange systems
- [UNDP Model Governance Framework for Digital Legal Identity Systems](https://www.governance4id.org/) - rights-based governance framework for digital legal identity as a foundational DPI component
- [UNESCO Digital Competency Framework](https://www.unesco.org/en/digital-competency-framework) - strengthens digital skills and institutional capacity in government for civil servants and policymakers

### Interoperability

- [DPI Global Data Exchange Directory](https://www.dpi.global/globaldpi/dataexchange) - country examples of data exchange platforms and related DPI implementations
- [GovStack Building Blocks Specification](https://govstack.gitbook.io/specification/) - technical specs for interoperable government services
- [GovStack Consent Building Block](https://govstack.gitbook.io/bb-consent/v/consent-1.0/) - specification for managing user consent and authorization across digital government services
- [GovStack Information Mediation Building Block](https://govstack.gitbook.io/bb-information-mediation) - data exchange and interoperability building block for secure service-to-service communication
- [GovStack Messaging Building Block](https://govstack.gitbook.io/bb-messaging/v/messaging-1.0/) - reusable messaging capability for notifications and communications in digital public services
- [GovStack Payments Building Block](https://govstack.gitbook.io/bb-payments/v/payments-1.0/) - payment orchestration specification for government service delivery
- [GovStack Registration Building Block](https://govstack.gitbook.io/bb-registration/v/registration-1.0/) - reusable registry capability for people, organizations, and service records
- [GovStack Scheduler Building Block](https://govstack.gitbook.io/bb-scheduler/v/scheduler-1.0/) - appointment and scheduling capability for public service workflows
- [GovStack Workflow Building Block](https://govstack.gitbook.io/bb-workflow/v/workflow-1.0.1/) - workflow orchestration specification for cross-agency digital services
- [OpenHIE Architecture](https://ohie.org/framework/) - health information exchange reference architecture
- [IHE Integration Profiles](https://www.ihe.net/resources/profiles/) - integration profiles for healthcare interoperability

### Prototyping & Implementation

- [X-Road Simulator Farm](https://github.com/paulo-amaral/xroad-simulator) - X-Road sandbox and reference architecture: a complete ecosystem (Central Server, test CA, Security Servers) on Docker Compose/Kubernetes with eID/e-KYC, citizen portal, observability, and test-driven development guides; originally built for the Government of Timor-Leste
- [GovStack Sandbox](https://sandbox.govstack.global/) - demonstration environment for developers to test GovStack architecture and the building-block approach
- [GovStack Sandbox Documentation](https://govstack.gitbook.io/sandbox/1.0.2-1) - technical walkthrough of the sandbox, APIs, emulators, adapters, and transaction flows
- [GovStack Use Case Simulation](https://simulation.govstack.global/) - interactive social cash transfer simulation showing how building blocks fit together in a digital service
- [GovStack Service Design Playbook](https://playbook.govstack.global/implementation/design-service) - hands-on guidance for mapping as-is services, user needs, journeys, and to-be digital service design
- [GovStack Building Block Software](https://govstack.global/software/) - product-agnostic catalogue for browsing open-source and proprietary software that implements GovStack Building Blocks, including compliance reports
- [UNDP DPI Approach Playbook](https://www.undp.org/sites/g/files/zskgke326/files/2023-08/undp-the-dpi-approach-a-playbook.pdf) - practical PDF playbook with checklists, assessment tools, case studies, and governance guidance for countries starting DPI
- [Deloitte Digital Public Infrastructure Playbook](https://www.deloitte.com/content/dam/assets-zone3/us/en/docs/industries/government-public-services/2024/in-ps-dpi-playbook-brand-noexp.pdf) - direct PDF playbook for DPI strategy, design, and implementation planning from a government and public services lens
- [UN 2.0: The Digital Public Infrastructure Approach](https://un-two-zero.network/contents/the-digital-public-infrastructure-approach-a-playbook/) - UN 2.0 catalogue entry for the DPI playbook, useful as a concise overview page before sharing the full PDF
- [UNDP Guide to Digital Participation Platforms 2025](https://www.undp.org/publications/guide-digital-participation-platforms-2025) - practical guide and platform matrix for inclusive civic engagement, consultation, and participatory democracy tools
- [World Bank Digital Agriculture Roadmap Playbook](https://connect4impact.worldbank.org/system/files/2026-03/Digital%20Agriculture%20Roadmap%20Playbook.pdf) - 2025 toolkit for developing country digital agriculture strategies and investment roadmaps
- [World Bank Fast Payments and Financial Market Infrastructure Toolkit](https://academy.worldbank.org/en/prosperity/fci/fast-payments-and-financial-market-infrastructure) - learning toolkit on fast payment systems, financial market infrastructure, and Project FASTT

### Procurement & Policy

- [CDPI DPI-as-a-Packaged Solution (DaaS)](https://docs.cdpi.dev/initiatives/dpi-as-a-packaged-solution-daas) - CDPI's approach to rapid DPI deployment (3–6 months) using pre-packaged open-source solutions, trained vendors, and policy templates; Trinidad and Tobago was the first country to go live with DaaS, rolling out verifiable credentials at national scale
- [UNICEF Venture Fund Guidance](https://www.unicef.org/innovation/venturefund) - how to fund and scale DPGs in low-income countries
- [Digital Square Global Goods Maturity Model](https://digitalsquare.org/global-goods-maturity-model) - maturity model for health digital tools
- [Open Source Policy Guide](https://github.com/todogroup/ospology) - policy frameworks and OSPO guidance for government open-source adoption
- [ITU Model Policy on Open Source](https://www.itu.int/) - ITU guidance for national open-source policies

---

## Organizations & Communities

### UN System & Multilaterals

| Organization | What they do |
|---|---|
| [Digital Public Goods Alliance (DPGA)](https://digitalpublicgoods.net/) | Defines and certifies DPGs |
| [UNICEF Office of Innovation](https://www.unicef.org/innovation/) | Funds DPGs and frontier tech for children |
| [UNDP Digital](https://www.undp.org/digital) | Digital transformation in 170+ countries |
| [ITU](https://www.itu.int/) | UN agency for ICTs |
| [World Bank Digital Development](https://www.worldbank.org/en/topic/digitaldevelopment) | Finances digital infrastructure |
| [World Bank Global DPI Program](https://www.worldbank.org/en/results/2026/05/06/global-digital-public-infrastructure-program) | Cross-sector DPI programme supporting digital ID, payments, and secure data sharing in 80+ countries |
| [UN OICT](https://unite.un.org/) | UN Office of ICT |

### Foundations & Alliances

| Organization | Focus |
|---|---|
| [50-in-5 Campaign](https://50in5.net/) | Country-led campaign to help 50 countries design, launch, and scale DPI components within five years |
| [Centre for Digital Public Infrastructure (CDPI)](https://cdpi.dev/) | Pro bono DPI advisory, architecture blueprints, DaaS rapid deployment, and open resources for country-scale DPI |
| [Digital Impact Alliance (DIAL)](https://digitalimpactalliance.org/) | Research on digital development |
| [Digital Square](https://digitalsquare.org/) | Grants for global digital health tools |
| [BMZ Digital.Global](https://www.bmz-digital.global/en/) | German Federal Ministry (BMZ) digital development programme - umbrella for GovStack, FAIR Forward (AI for development), atingi (digital skills), and Digital Transformation Centers |
| [Co-Develop Fund](https://www.codevelop.fund/) | Philanthropic funding for DPI in low-income countries - [publications](https://www.codevelop.fund/publications): evidence compendium, sector reports (health, agriculture, SIDS), and deployment guidance |
| [Gates Foundation](https://www.gatesfoundation.org/our-work/programs/global-growth-and-opportunity/inclusive-financial-systems) | Financial inclusion |
| [Omidyar Network](https://omidyar.com/) | Investment in DPI and open internet |
| [Rockefeller Foundation](https://www.rockefellerfoundation.org/) | Digital equity |

### Technical Communities

- [Global DPI Summit](https://www.globaldpisummit.org/) - annual convening for countries, implementers, funders, and experts working on safe and inclusive DPI
- [GovStack Community](https://www.govstack.global/) - people building reusable government building blocks
- [OpenHIE Community](https://ohie.org/) - health information exchange implementers worldwide
- [Open Source Ecosystem Enabler (OSEE)](https://www.undp.org/digital/osee) - ITU-UNDP initiative supporting open-source ecosystems, OSPOs, and sustainable digital public services
- [Open Source United](https://opensource.un.org/en/initiatives) - UN portal for open-source initiatives, including OSEE and open-source public sector collaboration
- [Digital Development Forum](https://www.digitaldevelopment.org/) - ICT4D community of practice
- [ICTworks](https://www.ictworks.org/) - good resource hub for digital development professionals

---

## Research & Reports

### Start Here

- [DPI-AI Framework: Building AI-Ready Nations through Digital Public Infrastructure](https://digitalpublicinfrastructure.ai/) - CDPI vision paper (2026) on embedding AI into DPI via AI Blocks, DPI Workflows, and Public Agents; CC BY 4.0
- [The Agentic State: Rethinking Government for the Era of Agentic AI](https://agenticstate.org/) - vision paper (2025, Global GovTech Centre / World Bank) covering AI in public services, workflows, procurement, governance, and crisis response; launched at Tallinn Digital Summit
- [Government Trends 2025: Built to Deliver](https://www.deloitte.com/gr/en/Industries/government-public/about/government-trends-2025.html) - Deloitte report on nine trends advancing government's capacity to deliver large-scale priorities amid rising citizen expectations, technology shifts, and implementation constraints
- [Deloitte Digital Public Infrastructure Playbook](https://www.deloitte.com/content/dam/assets-zone3/us/en/docs/industries/government-public-services/2024/in-ps-dpi-playbook-brand-noexp.pdf) - DPI playbook PDF for government teams and advisors planning national or sector digital public infrastructure initiatives
- [2025 State of Digital Public Infrastructure Report](https://www.ucl.ac.uk/bartlett/publications/2025/nov/2025-state-digital-public-infrastructure-report) - UCL IIPP baseline report on DPI measurement, prevalence, and maturity across 210 countries
- [2025 State of the Digital Public Goods Ecosystem](https://www.digitalpublicgoods.net/blog/2025-dpg-ecosystem-report) - DPGA report on verified DPG growth, DPG-for-DPI value, financing, governance, and ecosystem priorities
- [A Digital Public Infrastructure Approach for the Agriculture Sector](https://connect4impact.worldbank.org/system/files/2026-02/DPI-Approach-for-Agriculture-Sector_Final_.pdf) - World Bank sector paper on applying DPI building blocks to farmer registries, data exchange, advisory services, traceability, and agri-finance
- [Accelerating the SDGs Through Digital Public Infrastructure](https://www.undp.org/publications/accelerating-sdgs-through-digital-public-infrastructure-compendium-potential-digital-public-infrastructure) - UNDP compendium mapping DPI and DPI-like solutions to all 17 SDGs
- [Digital Public Infrastructure and Development: A World Bank Group Approach](https://documents1.worldbank.org/curated/en/099031025172027713/pdf/P505739-84c5073b-9d40-4b83-a211-98b2263e87dd.pdf) - World Bank Digital Transformation White Paper, Vol. 1 (2025)
- [Digital Public Infrastructure for Digital Governments](https://www.oecd.org/content/dam/oecd/en/publications/reports/2024/12/digital-public-infrastructure-for-digital-governments_11fe17d9/ff525dc8-en.pdf) - OECD paper on DPI as a foundation for digital government services, trust, and interoperability
- [The Case for a New Digital Bretton Woods](https://www.bu.edu/gdp/) - Boston University Global Development Policy Center
- [The Economics of Digital Public Infrastructure](https://dial.global/research/economics-of-digital-public-infrastructure/) - DIAL / Co-Develop research on DPI's economic case for equitable growth
- [The Human and Economic Impact of Digital Public Infrastructure](https://www.undp.org/publications/human-and-economic-impact-digital-public-infrastructure) - UNDP/Dalberg study estimating DPI impact across finance, justice, and climate in 70 LMICs
- [Rethinking Digital Public Infrastructure](https://www3.weforum.org/docs/WEF_Rethinking_Digital_Public_Infrastructure.pdf) - World Economic Forum
- [Digital Public Infrastructure and Democracy](https://omidyarnetwork.com/) - Omidyar Network
- [The case for Nature ID](https://www.undp.org/publications/case-nature-id-how-digital-public-infrastructure-can-catalyze-nature-and-climate-action) - UNDP paper on environmental data exchange DPI for climate action, biodiversity, traceability, and green finance

### Impact Evidence

- [DHIS2: 30 Years of Health Information Infrastructure](https://dhis2.org/impact/) - country-level impact across 100+ countries
- [MOSIP Country Implementations](https://mosip.io/country.php) - national ID deployments across Africa and Asia
- [Mojaloop Impact Report](https://mojaloop.io/) - financial inclusion through open payments
- [India Stack Impact](https://indiastack.org/) - 1.3B identities, $2T+ in UPI transactions annually

### Policy

- [OECD Going Digital Policy Notes](https://www.oecd.org/going-digital/policy-notes.htm) - country-specific digital transformation guidance
- [AfDB Digital Transformation Strategy](https://www.afdb.org/en/topics-and-sectors/topics/digital-transformation) - Africa's digital infrastructure priorities
- [G20 DPI Framework](https://www.g20.org/) - G20 DPI commitments and principles
- [OECD Government at a Glance 2025: Digital Public Infrastructure](https://www.oecd.org/en/publications/government-at-a-glance-2025_0efd0bcd-en/full-report/digital-public-infrastructure_1cee4220.html) - comparative OECD chapter on digital identity, data exchange, interoperability, and public service delivery
- [Deloitte Government Trends 2025](https://www.deloitte.com/gr/en/Industries/government-public/about/government-trends-2025.html) - annual government trends report focused on delivery capacity, agile governance, citizen expectations, and technology-enabled public sector transformation

### Digital Workforce & Inclusion

- [GovStack Inclusive Design Whitepaper](https://www.govstack.global/app/uploads/2024/06/2024_GovStack_Inclusive-Design-Whitepaper.pdf) - guidance for gender-responsive, accessible, and inclusive digital government service design
- [ITU Facts and Figures 2025: Gender Digital Divide](https://www.itu.int/itu-d/reports/statistics/2025/10/15/ff25-the-gender-digital-divide/) - current ITU data on the gap between women and men in internet use and digital access
- [Mozambique Digital Economy](https://www.trade.gov/country-commercial-guides/mozambique-digital-economy) - country commercial guide overview of Mozambique's digital economy, ICT market, and e-government context
- [UN Women - Power On](https://www.unwomen.org/en/news-stories/explainer/2023/02/power-on-how-we-can-supercharge-an-equitable-digital-future) - explainer on closing gender gaps in digital access, skills, leadership, and online safety
- [W3C WAI Accessibility Principles](https://www.w3.org/WAI/fundamentals/accessibility-principles/) - web accessibility principles and references to WCAG, UAAG, ATAG, and WAI-ARIA for inclusive public services
- [WEF Global Gender Gap Report 2025](https://www.weforum.org/publications/global-gender-gap-report-2025/) - annual benchmark on gender gaps across economic participation, education, health, and political empowerment
- [Where is Digital Youth Work? Policy Invisibility and the Case for Recognition](https://dywrhubreport2026.netlify.app/) - University of Leeds / INCLUDE+ Network (2026); reviews 800+ government bodies and 26 policies to show how youth workers - the most effective digital inclusion practitioners - are systematically excluded from policy and funding

---

## Courses & Learning

### Free Courses

| Course | Provider | Level |
|--------|----------|-------|
| [DPI Academy](https://www.undp.org/digital/academy) | UNDP | Beginner to Intermediate |
| [ITU Academy](https://academy.itu.int/) | ITU | All levels |
| [DHIS2 Academy](https://dhis2.org/academy/) | DHIS2 | Beginner to Advanced |
| [GovStack Learning Path](https://govstack.global/) | GovStack | Technical |
| [Digital Principles e-Learning](https://digitalprinciples.org/principles/) | DIAL | Beginner |
| [ODK Documentation](https://docs.getodk.org/) | ODK | Technical |

### Certifications

- [ISACA CGEIT](https://www.isaca.org/credentialing/cgeit) - governance of enterprise IT, recognized in the public sector
- [Project DPG Certification](https://digitalpublicgoods.net/) - understanding the DPG standard and certification process

---

## Field Notes

Things learned working in the field that don't appear in any framework document. Built from implementations with UNICEF, UNDP, and government teams across Timor-Leste, the Pacific, and fragile states.

| Note | Topics |
|------|--------|
| [Timor-Leste and the Pacific](docs/field-notes/timor-leste-pacific.md) | Fragile states, ministry alignment, identifiers, offline tools |
| [Design & Architecture](docs/field-notes/design-architecture.md) | HCD, service blueprints, user journeys, TOGAF |
| [Offline-First & Last Mile](docs/field-notes/offline-first.md) | Connectivity, sync, device testing, 2G |
| [Digital Divide, AI Divide & Inclusion](docs/field-notes/digital-divide-inclusion.md) | Gender, disability, language, AI divide |
| [Emerging Technologies](docs/field-notes/emerging-technologies.md) | Drones, AgriTech, AI, data readiness |
| [Policies, Standards & Laws](docs/field-notes/policies-standards-laws.md) | Legal alignment, data protection, standards, governance |
| [Common Mistakes](docs/field-notes/common-mistakes.md) | Vendor lock-in, sustainability, interoperability |

 [Browse all field notes](docs/field-notes/README.md)

---

## Contributing

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

<sub>Content is CC0 - public domain. All software listed is open source. See each project's license for details.</sub>

</div>

---

<div align="center">

If this list was useful, star it and pass it on.

[paulo-amaral.github.io](https://paulo-amaral.github.io/)

*Made with  in the  island*

</div>
