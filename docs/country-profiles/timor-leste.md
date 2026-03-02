# Timor-Leste — DPI Profile

## Overview

Timor-Leste (East Timor) is one of Asia's youngest nations, gaining independence in 2002. With a population of approximately 1.3 million across a mountainous terrain and 13 municipalities, the country faces significant infrastructure challenges: limited electricity coverage, sparse internet connectivity, and a public workforce still developing digital skills.

Despite these constraints, Timor-Leste has made meaningful progress in specific DPI domains — particularly in health information management, child protection data systems, and government administrative digitization. The country offers an important case study of **DPI in fragile state contexts**: where ambition must be calibrated to infrastructure reality, and where UN agencies and international partners play an outsized role in both funding and implementation.

## DPI Stack

| Layer | Solution | Status | Implementing Partners |
|-------|----------|--------|----------------------|
| Health HMIS | [e-SISCA](https://www.moh.gov.tl/) | Live (partial) | MoH, WHO, UNFPA |
| Child Protection MIS | [CPMIS](https://github.com/) | Pilot → Rollout | MSSI, MoJ, MoI, MoE, UNICEF |
| Civil Registration | RDTL Civil Registry | Partial digital | Ministry of Justice |
| Tax & Revenue | SIGTAS | Live | Ministry of Finance |
| Budget Management | FREEBALANCE | Live | Ministry of Finance |
| Government Portal | [RDTL.tl](https://www.rdtl.tl/) | Partial | MICS |
| Community Health | SISCA (paper + digital) | Partial | MoH, WHO |

## CPMIS — Child Protection Management Information System

The **CPMIS** (Child Protection MIS) is a purpose-built data pipeline developed with UNICEF support in 2025–2026 to monitor child protection indicators across 4 ministries:

| Ministry | Indicator Monitored |
|----------|---------------------|
| MSSI (Social Solidarity) | Regulations & SOPs — Lei N.º 9/2022 |
| MoJ (Justice) | Child-Friendly Justice Frameworks |
| MoI / PNTL (Interior/Police) | Child Homicide Rate per 100,000 |
| MoE (Education) | School Attendance Rate, ages 6–18 |

**Technical stack:**
- **Data collection:** KoboToolbox (EU instance) with custom XLSForms per ministry
- **Pipeline:** Google Apps Script (daily automated pull via KoboToolbox API)
- **Storage:** Google Sheets (30-column flat schema, ministry-specific tabs)
- **Visualization:** Looker Studio dashboard
- **Notifications:** Automated email alerts for new submissions and deadline reminders

**Key design decisions:**
- Deliberately simple stack (no custom server infrastructure) to enable government self-hosting post-project
- XLSForms designed by UNICEF CP team in collaboration with focal points from each ministry
- Automated deadline reminder system (T-7, T-2, T-0 days) to drive compliance with quarterly reporting cycle

## Open-Source Tools in Use

- [KoboToolbox](https://www.kobotoolbox.org/) — Primary data collection platform across humanitarian programs
- [DHIS2](https://dhis2.org/) — Health information system (MoH, limited deployment)
- [Primero](https://www.primero.org/) — Child protection case management (UNICEF-supported rollout)
- [Google Apps Script](https://developers.google.com/apps-script) — Automation layer for CPMIS pipeline
- [Looker Studio](https://lookerstudio.google.com/) — Dashboard visualization (free tier)

## Key Milestones

- **2002:** Independence — digital infrastructure built from near-zero
- **2010s:** e-SISCA health information system piloted in select municipalities
- **2016:** National Statistics Directorate (DNE) begins digital data collection pilots
- **2022:** Lei N.º 9/2022 — Child Protection Law enacted, creating mandatory reporting framework
- **2024:** UNICEF CP Section begins CPMIS design with 4 ministries
- **2025:** CPMIS KoboToolbox forms deployed and tested with ministry focal points
- **2026:** CPMIS full rollout — automated quarterly reporting pipeline operational

## Lessons Learned

These lessons reflect direct field experience from CPMIS implementation:

**Infrastructure constraints shape design:**
- Reliable internet is unavailable in many municipality offices. Forms must work offline and sync when connectivity is available. KoboToolbox's offline-capable mobile app is essential.
- Do not design for smartphone-first. Many focal points use shared desktop computers or basic Android phones on 3G.

**Organizational complexity exceeds technical complexity:**
- Getting 4 ministries to agree on a common data schema took longer than building the entire pipeline.
- Each ministry has different reporting cultures, capacity levels, and political priorities. One-size-fits-all training does not work.

**Consistency beats sophistication:**
- A simple Google Sheets pipeline that works reliably every day delivers more value than a sophisticated HMIS that requires constant IT support.
- Automated email reminders (with deadline tracking) doubled reporting compliance compared to manual follow-up.

**Enforce data standards at source:**
- Cycle ID format mismatches between form calculation (`MSSI_2026_q1`) and backend logic (`CPMIS_2026_q1`) caused entire quarters of data to appear "missing." Data governance decisions made in the form must match backend logic exactly.

**Plan for ownership transitions:**
- Every technical decision should be evaluated against: "Can the MSSI IT team maintain this in 3 years without UNICEF support?"
- Google Workspace tools (Sheets, Apps Script, Looker Studio) were chosen specifically because government staff already have Google accounts and basic familiarity.

## Challenges and Gaps

- **No foundational digital ID:** Timor-Leste lacks a functioning national ID system. This limits cross-program beneficiary verification.
- **Limited local tech capacity:** Very few ICT professionals are available for government digital initiatives. All systems must be designed for minimal ongoing technical support.
- **Donor-dependent sustainability:** Most digital systems are donor-funded with unclear government operational budgets post-project.
- **Language fragmentation:** Official languages (Tetum, Portuguese) plus 16+ local languages create localization challenges for any citizen-facing system.
- **Single-country scale limits reuse:** Solutions designed for 1.3M people are not economically interesting for large DPG vendors, requiring custom or simplified implementations.

## References

- [UNICEF Timor-Leste](https://www.unicef.org/timorleste/)
- [Government of Timor-Leste — RDTL](https://www.rdtl.tl/)
- [Ministry of Health — MoH](https://www.moh.gov.tl/)
- [MSSI — Ministry of Social Solidarity & Inclusion](https://www.mssi.gov.tl/)
- [World Bank: Timor-Leste Digital Economy](https://www.worldbank.org/en/country/timor-leste)
- [UNDP Timor-Leste Digital Transformation](https://www.undp.org/timor-leste)
