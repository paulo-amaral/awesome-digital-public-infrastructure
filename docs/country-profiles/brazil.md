# Brazil — DPI Profile

## Overview

Brazil has developed one of Latin America's most sophisticated Digital Public Infrastructure ecosystems. The country's DPI is anchored by three pillars: **PIX** (instant payments, 2020), **GOV.BR** (unified digital identity and government services portal), and **Open Finance** (open banking framework mandated by the Central Bank). Together they serve 215 million people.

Brazil is notable for combining **regulatory mandates** with **technical openness** — PIX's interoperability was mandated by the Central Bank, and the Open Finance framework requires all financial institutions to participate. This creates network effects that purely voluntary approaches rarely achieve.

## DPI Stack

| Layer | Solution | Launch | Scale |
|-------|----------|--------|-------|
| Instant Payments | [PIX](https://www.bcb.gov.br/estabilidadefinanceira/pix) | Nov 2020 | 140M+ users, 4B+ monthly txn |
| Digital Identity | [GOV.BR](https://www.gov.br/) | 2019 | 150M+ accounts |
| Open Finance | [Open Finance Brasil](https://openfinancebrasil.org.br/) | 2021 | 40M+ consents |
| Health Records | [Conecte SUS](https://conectesus.saude.gov.br/) | 2021 | 200M+ records |
| Electronic Voting | [e-Voting (Urna Eletrônica)](https://www.tse.jus.br/) | 1996 | 156M voters |
| Digital Signature | [e-Title / e-CPF](https://www.iti.gov.br/) | 2001 | ICP-Brasil PKI |
| Social Registry | [CadÚnico](https://www.gov.br/pt-br/servicos) | 2001 | 90M+ beneficiaries |

## Open-Source Tools and Specifications

- [PIX API Specification](https://www.bcb.gov.br/estabilidadefinanceira/pix) — Open API standards for PIX integration (mandatory for all Brazilian banks)
- [Open Finance Brasil APIs](https://openfinancebrasil.org.br/) — Open API specifications for the Brazilian Open Finance ecosystem
- [Apache Fineract](https://fineract.apache.org/) — Open core banking platform used by Brazilian fintechs building on PIX
- [Mojaloop](https://mojaloop.io/) — PIX's architecture influenced subsequent open payment systems globally
- [DHIS2](https://dhis2.org/) — Health information system used in Brazilian states for epidemiological surveillance

## Key Milestones

- **1996:** Electronic voting system introduced — Brazil becomes world leader in digital elections
- **2001:** ICP-Brasil PKI framework established — legal digital signatures
- **2001:** CadÚnico social registry launched — foundational dataset for social programs
- **2019:** GOV.BR unified portal launches — single login for all federal services
- **Nov 2020:** PIX goes live — instant 24/7 payments, free for individuals, interoperable across all banks
- **2021:** Open Finance Phase 1 — mandatory data sharing between financial institutions
- **2022:** PIX reaches 100M users — fastest payment system adoption in history
- **2023:** PIX Automático (recurring payments) and PIX Internacional in development

## Lessons Learned

- **Regulation as the accelerator:** Making PIX participation mandatory for large banks created instant critical mass. Voluntary approaches had stalled for years.
- **Free at the point of use for individuals:** PIX is free for individuals (banks may charge businesses). This drove adoption faster than any marketing campaign.
- **Design for the unbanked:** PIX onboarding was designed to work through digital bank accounts (including those with no minimum balance), bringing previously unbanked populations into the formal system.
- **Open Finance requires phasing:** Brazil implemented Open Finance in 4 phases over 2+ years. Trying to do everything at once would have failed.
- **Legacy data as DPI:** CadÚnico's 20 years of social registry data became the backbone for emergency COVID cash transfers to 65M+ families — proof that data infrastructure has long-term compounding value.

## References

- [Banco Central do Brasil — PIX](https://www.bcb.gov.br/estabilidadefinanceira/pix)
- [Open Finance Brasil](https://openfinancebrasil.org.br/)
- [GOV.BR Portal](https://www.gov.br/)
- [BIS: PIX — The Brazilian Instant Payment Ecosystem](https://www.bis.org/)
- [World Bank: Brazil Digital Economy Report](https://www.worldbank.org/en/country/brazil)
- [IDB: Lessons from Brazil's Digital Financial Infrastructure](https://www.iadb.org/)
