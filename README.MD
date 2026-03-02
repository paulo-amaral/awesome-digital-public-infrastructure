# Awesome Digital Public Infrastructure 

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re) [![Contributions Welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg)](CONTRIBUTING.md) [![Last Updated](https://img.shields.io/github/last-commit/paulo-amaral/awesome-digital-public-infrastructure)](https://github.com/paulo-amaral/awesome-digital-public-infrastructure/commits/main) [![Latest Release](https://img.shields.io/github/v/release/paulo-amaral/awesome-digital-public-infrastructure?label=release)](https://github.com/paulo-amaral/awesome-digital-public-infrastructure/releases) [![Buy Me A Coffee](https://img.shields.io/badge/Buy%20me%20a%20coffee-support-orange?style=flat&logo=buy-me-a-coffee&logoColor=white)](https://www.buymeacoffee.com/paulosecur5)

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
- [💼 Jobs & Opportunities](#jobs--opportunities)
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

- [Digital Public Infrastructure and Development: A World Bank Group Approach](https://documents1.worldbank.org/curated/en/099031025172027713/pdf/P505739-84c5073b-9d40-4b83-a211-98b2263e87dd.pdf) — World Bank Digital Transformation White Paper, Vol. 1 (2025)
- [The Case for a New Digital Bretton Woods](https://www.bu.edu/gdp/) — Boston University Global Development Policy Center
- [DPI: A Moonshot for Equitable Growth](https://www.co-develop.net/dpi-moonshot) — Co-Develop Fund, 2022
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

## 💼 Jobs & Opportunities

### 🔍 Where to Look

| Platform | What's there |
|----------|-------|
| [DevNetJobs](https://www.devnetjobs.org/) | International development tech roles |
| [ReliefWeb Jobs](https://reliefweb.int/jobs) | Humanitarian and development positions |
| [UN Careers](https://careers.un.org/) | UN Secretariat and agency roles |
| [UNICEF Careers](https://www.unicef.org/careers/) | ICT and innovation roles |
| [ICTworks Job Board](https://www.ictworks.org/category/jobs/) | ICT for development |
| [LinkedIn](https://www.linkedin.com/jobs/) | Search: DPI, DPG, GovTech, Digital Transformation |

### 💰 Fellowships, Grants & Funding

| Opportunity | Who it's for |
|-------------|--------------|
| [UNICEF Venture Fund](https://www.unicef.org/innovation/venturefund) | DPG startups in low-income countries, no equity taken |
| [Digital Square Open Calls](https://digitalsquare.org/opencalls) | Grants for global digital health tools |
| [DIAL Fellowship](https://dial.global/) | Digital development practitioners |
| [Co-Develop Country Grants](https://www.co-develop.net/) | Governments implementing DPI |

---

## 🏕️ Field Notes

Things I learned working in the field that don't appear in any framework document.

### 🌴 From Timor-Leste and the Pacific

- **📶 Start with what works, not what's ideal.** In fragile states, KoboToolbox running on 3G beats a complex HMIS that needs a reliable server and trained IT staff. Build up from there.
- **🤝 The technology is the easy part.** Getting four ministries to agree on a common data schema took longer than building the entire pipeline. Budget time for this — seriously.
- **🔑 Agree on identifiers before you start.** Cycle IDs like `MSSI_2026_q1` need to match across the form, the pipeline, and the reporting logic from day one. Fixing this later is painful and expensive.
- **📄 Always design for PDF.** Even with a live dashboard, senior government officials will ask for a PDF by email. Both channels need to work.
- **🌊 The Pacific is not one context.** Fourteen island nations spread across millions of km² means offline-capable tools, cross-jurisdiction data agreements, and very limited local technical capacity. Generic solutions rarely fit.

### 🧑‍🤝‍🧑 Design & Architecture

- **👤 People first, always.** Human-Centered Design (HCD) is not optional. Run user research before writing a single requirement. The focal point filling in a form at 3G speed in a municipal office is your real user — not the minister who sees the dashboard.
- **🗺️ Service blueprints before system design.** Map the as-is service end-to-end before touching any technology: who does what, when, with what information, and where it breaks. One day with frontline staff reveals more than a month of requirements documents.
- **🛤️ User journeys are your north star.** Walk the full journey for each persona — focal point, programme officer, ministry director. Build the to-be journey first. Every technical decision should trace back to it.
- **🏗️ TOGAF keeps the architecture conversation honest.** Even a lightweight pass through the ADM layers — Business → Data → Application → Technology — stops teams jumping straight to tools. It forces alignment on *what problem* you are solving before anyone debates *which platform* to use.

### 📵 Offline-First & Last Mile

- **Design offline-first, not offline-compatible.** There is a difference. Offline-compatible means someone added a sync button after launch. Offline-first means every interaction was designed assuming no connectivity — data queues locally, conflicts are resolved deterministically, and the user never sees a spinner. In fragile and rural contexts, this is the baseline, not an edge case.
- **The last-mile problem is not a technical problem.** In most countries it is already known, costed, and budgeted — and still unresolved after a decade because the economics do not work for private operators and the political will for public investment is absent. Do not design DPI that depends on last-mile connectivity being solved first. Degrade gracefully: offline collection, async sync, SMS fallback, paper backup. The system that works on 2G today delivers more value than the one waiting for fibre in 2030.
- **Test on the actual device.** A form that loads in 2 seconds on Chrome degrades to 45 seconds on a shared Android 8 phone in a municipal office. Test on the hardware your users actually have, in the connectivity conditions they actually face. This single practice eliminates more UX problems than any amount of user research done remotely.

### ⚖️ Digital Divide, AI Divide & Inclusion

- **The digital divide is not disappearing — it is replicating.** As foundational DPI (identity, payments, data exchange) becomes standard, a second layer of exclusion is forming around those who cannot use it: people without smartphones, without literacy, without the time or trust to engage with digital systems. DPI design that ignores this layer does not solve the divide — it moves the cutoff point.
- **The AI divide is the digital divide at speed.** Countries and communities that lack clean, structured, governed data will not be able to use AI-enhanced public services — not because they lack AI, but because AI requires data infrastructure that takes years to build. If DPI is not deployed with data quality and governance as first-class concerns, the AI divide widens with every model release.
- **Gender is a design variable, not a disclaimer.** Women in many low-income contexts have lower mobile ownership rates, lower literacy rates, and face social constraints on independent digital access. A DPI system that is nominally accessible but practically unusable for half the population is not a success. Collect disaggregated data by gender from day one. Run user research with women separately. Design for the constrained case.
- **Disability and language are not edge cases.** In Pacific and Southeast Asian contexts, populations speak dozens of languages, including languages with no digital keyboard support. Screen readers are rare. Form logic that requires reading long instructions excludes a significant share of users. Build with the hardest-to-reach user in mind — everyone else is easier.

### 🌐 Emerging Technologies

- **Drones are DPI infrastructure in disguise.** In remote or island geographies, drone delivery of samples, medicines, and data collection hardware is already operational (Rwanda, Vanuatu). The DPI layer — routing, identity, logistics data — is what makes it scale. Design for drone integration the same way you design for mobile: as a channel, not a novelty.
- **AgriTech requires ground truth, literally.** Satellite imagery, remote sensing, and AI crop monitoring are powerful — but they fail without local ground-truth data from farmers. The DPI layer that connects field agents, mobile forms, and satellite APIs is where the value is created. Tools like ODK, KoboToolbox, and DHIS2 are already being used for agricultural data pipelines.
- **AI works when the data does.** Generative AI and predictive models for public services only work if the underlying data infrastructure is clean, consistent, and governed. Before deploying AI on top of DPI, ask: Is the data collected consistently? Are identifiers stable? Is there a data steward? Most AI failures in development contexts are data failures, not model failures.
- **Emerging tech follows the same rule as everything else.** The question is never "is this technology exciting?" The question is "does this solve a real problem my users have, and can it be maintained by the people who will inherit it?" A drone corridor in Rwanda works because there is operational capacity behind it. A blockchain pilot in a fragile state usually does not.

### 🏛️ Policies, Standards & Laws Alignment

- **DPI without legal alignment is a liability, not an asset.** Before deploying any system that handles personal data, verify that a data protection law exists and applies — and that someone is responsible for enforcing it. If no framework exists, the DPI creates obligations nobody is prepared to fulfil. Map the legal landscape first: data protection, electronic transactions, cybersecurity, sector-specific regulations (health, finance, education), and any binding regional commitments (AU Data Policy Framework, ASEAN Digital Masterplan, EU adequacy decisions).
- **Technology consistently outpaces legislation by years.** The DPI architect must flag legal gaps as implementation risks, not afterthoughts. A system that is technically complete but legally ungrounded will be shut down, misused, or quietly abandoned when political winds shift. Budget time for legal review alongside technical review.
- **Standards alignment determines whether a pilot can ever scale.** Interoperability specifications are not optional extras — they are the difference between a system that talks to others and one that dies in isolation. Before committing to a technical architecture, check alignment with: [GovStack Building Blocks](https://specs.govstack.global/), [OpenHIE Reference Architecture](https://ohie.org/), [FHIR](https://www.hl7.org/fhir/) (health), [OpenID Connect](https://openid.net/) (identity), and sector-specific standards. Non-compliance discovered late costs 10× more to fix than compliance designed in from the start.
- **Existing laws are often ambiguous about digital systems.** A data protection law written in 2005 may not cover biometric collection, AI-assisted decision-making, or cross-border data flows in cloud infrastructure. Legal ambiguity is itself a risk — document every assumption about legal interpretation and get written guidance from the relevant authority before going live.
- **Regional and multilateral commitments create hidden obligations.** A country that has signed the AU Data Policy Framework, acceded to the Budapest Convention on Cybercrime, or is seeking EU adequacy has binding obligations that must be reflected in DPI design. These are not bureaucratic obstacles — they are the legal foundation that protects the system's legitimacy long-term.

### ⚠️ Common Mistakes

| What goes wrong | How it looks | How to avoid it |
|--------|-------------------|--------------|
| **Vendor lock-in as DPI** | "Open" solutions with closed APIs | Check for open APIs and exportable data before you sign anything |
| **Digital-first, everyone else later** | 30-40% of users have no smartphone | Build for USSD, IVR, and in-person from the start |
| **No sustainability plan** | System dies when the donor project ends | Budget for operations before features |
| **Interoperability as an afterthought** | Two systems that can't talk to each other | Design the integration architecture first |
| **Collecting data without governance** | Data piles up with no privacy framework | Governance before collection |
| **Copying India Stack** | Assuming what worked at 1.4B scale fits a country of 1.3M | Adapt to local context — legal, political, and capacity |

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
