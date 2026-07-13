# Cambodia - DPI Profile

## Overview

Cambodia (population ~17 million) has become one of Southeast Asia's most instructive DPI case studies. Rather than building from scratch, it adapted proven open-source components: its national data exchange layer, CamDX, is a direct adaptation of Estonia's X-Road, making Cambodia the first ASEAN country to deploy a nationwide government data exchange based on the Estonian model. Its central bank payment system, Bakong, runs on the open-source Hyperledger Iroha blockchain and now processes transaction volumes exceeding 300% of GDP.

Cambodia is also becoming a **DPI exporter**. Its document verification platform, verify.gov.kh, won Gold at the ASEAN Digital Awards 2024 and the UN Public Service Award 2026, and has been officially launched in Timor-Leste, with implementations underway in Laos and the Philippines. This South-South transfer reverses the usual donor-to-recipient flow of government technology.

## DPI Stack

| Layer | Solution | Status | Open Source? |
|-------|----------|--------|-------------|
| Data Exchange | [CamDX](https://camdx.gov.kh/) | Live (~20 services) | Yes (X-Road adaptation) |
| Digital ID / eKYC | [CamDigiKey](https://camdx.gov.kh/docs/open-api/ekyc) | Live | Partial (runs on CamDX) |
| Payments | [Bakong](https://bakong.nbc.gov.kh/) | Live | Yes (Hyperledger Iroha) |
| Document Verification | [verify.gov.kh](https://verify.gov.kh/) | Live, exported regionally | Blockchain-based |
| Business Registration | Online Business Registration (single portal on CamDX) | Live | Built on CamDX |

## CamDX - Cambodia Data Exchange

CamDX was developed and is operated by the **Techo Startup Center**, a delivery unit under the Ministry of Economy and Finance. Its Executive Director, Dr. Nguonly Taing, initiated the project after a 2019 study visit to Estonia, and the platform was deployed in 2020.

The launch use case was **online business registration**: before CamDX, multi-ministry approvals took 30 to 60 days; the single portal consolidated them into one flow. Around 20 government services now run on the exchange, and open eKYC services alone have processed on the order of 1 million transaction requests per month, serving banks and microfinance institutions from a unified data source.

**CamDigiKey**, the authentication and eKYC app operated on CamDX, lets users authenticate to any integrated government portal by scanning a QR code. It combines AI facial recognition and liveness detection with OCR extraction from Cambodian national ID cards and passports.

In November 2022, UNDP and partners recognized CamDX as the "open source adaptation of the year."

## Bakong - Blockchain-Based Payments

The National Bank of Cambodia (NBC) launched Bakong in October 2020, developed with the Japanese firm Soramitsu on the open-source **Hyperledger Iroha** framework. The NBC runs the core system and delegates payment gateways to commercial banks and financial institutions; end users connect through those gateways. Bakong supports fiat-backed digital representations of both the Khmer riel and the US dollar, and one of its stated policy goals is to promote riel usage in a heavily dollarized economy.

Growth has been steep: by 2023, the NBC reported 19.5 million accounts opened in total (many reached indirectly through member bank apps). In 2024, Bakong processed 608 million transactions worth US$104.8 billion, roughly 330% of Cambodia's GDP and a 95% increase over 2023. Cross-border QR payments with China's UnionPay launched in March 2023.

## verify.gov.kh - Document Verification as an Export

Developed by the Ministry of Post and Telecommunications (MPTC) using blockchain, AI, and hybrid cloud infrastructure, verify.gov.kh authenticates government-issued documents via QR codes.

- **2024:** Gold Medal, ASEAN Digital Awards (Public Sector category, Singapore), selected among 125 submissions from the 10 ASEAN member states.
- **2026:** UN Public Service Award for transparency and accountability.
- **Regional adoption:** Officially launched in Timor-Leste; implementations underway in Laos and the Philippines; discussions with Bangladesh.

## Open-Source Tools in Use

- [X-Road](https://x-road.global/) - foundation of CamDX, the national data exchange layer
- [Hyperledger Iroha](https://www.lfdecentralizedtrust.org/case-studies/soramitsu-case-study) - blockchain framework underlying Bakong

## Key Milestones

- **2019:** Techo Startup Center study visit to Estonia; CamDX design begins
- **2020:** CamDX deployed with online business registration as the anchor use case
- **2020 (October):** Bakong launched by the National Bank of Cambodia
- **2021:** Digital Economy and Society Policy Framework 2021–2035 adopted
- **2022:** Digital Government Policy 2022–2035 published (10 strategies, 83 priority actions); CamDX named UNDP "open source adaptation of the year"
- **2023:** Bakong cross-border QR payments with UnionPay (March)
- **2024:** verify.gov.kh wins Gold at ASEAN Digital Awards; Bakong volume reaches US$104.8 billion
- **2026:** verify.gov.kh wins UN Public Service Award; launched in Timor-Leste, rollouts in Laos and the Philippines

## Lessons Learned

**Adapt proven DPGs instead of building from scratch:**
- CamDX reused X-Road's architecture and got a national exchange layer live within roughly a year of the 2019 Estonia visit. The cost and time savings of adaptation over greenfield development are the core of the story.

**Anchor the exchange layer to one painful use case:**
- Business registration (30–60 day waits collapsed into a single portal) gave CamDX immediate, visible value. Services and eKYC integrations followed once the rail existed.

**A startup-style delivery unit works inside government:**
- The Techo Startup Center sits under the Ministry of Economy and Finance but operates with startup delivery practices. This mirrors patterns like India's NPCI and Estonia's RIA: a focused technical unit with a government mandate.

**Central-bank-operated rails with delegated access:**
- Bakong's tiered model (NBC runs the core, banks run the gateways) achieved mass reach without the central bank serving consumers directly.

**DPI can be an export product:**
- verify.gov.kh moving to Timor-Leste, Laos, and the Philippines shows that a lower-middle-income country can produce DPI that neighbors adopt, a South-South transfer pattern worth watching.

## Challenges and Gaps

- **Data protection law still pending:** Cambodia released its first comprehensive draft Law on Personal Data Protection in July 2025, modeled largely on the GDPR, but as of early 2026 it had not yet been enacted. DPI adoption is running ahead of the legal safeguards framework.
- **Dollarization:** Bakong's dual-currency design reflects a heavily dollarized economy; promoting riel usage remains a long-term policy goal rather than an achieved outcome.
- **Account figures overstate unique users:** Reported Bakong account totals (19.5 million in a country of 17 million) include indirect accounts through member bank apps, so unique-user penetration is lower than headline numbers suggest.
- **Connectivity and digital-divide gaps:** As in most of the region, rural connectivity and digital literacy constrain how far QR-based services reach beyond urban centers.

## References

- [CamDX - Cambodia Data Exchange](https://camdx.gov.kh/)
- [X-Road case study: CamDX is Cambodia's national data exchange solution](https://x-road.global/xroad-case-studies-library/2024/10/21/camdx-is-cambodias-national-data-exchange-solution-and-its-based-on-x-road)
- [OECD OPSI: CamDX](https://oecd-opsi.org/innovations/camdx-2/)
- [Bakong White Paper - National Bank of Cambodia (PDF)](https://bakong.nbc.gov.kh/download/NBC_BAKONG_White_Paper.pdf)
- [Soramitsu: Cambodia implements a digital currency](https://soramitsu.co.jp/cambodia-bakong/)
- [Hyperledger case study: National Bank of Cambodia](https://www.lfdecentralizedtrust.org/case-studies/soramitsu-case-study)
- [MPTC: verify.gov.kh wins Gold in ASEAN Digital Awards 2024](https://mptc.gov.kh/en/2024/02/cambodias-verify-gov-kh-document-verification-platform-wins-gold-in-asean-digital-awards-2024/)
- [MPTC: verify.gov.kh wins United Nations Public Service Award 2026](https://mptc.gov.kh/en/2026/06/press-release-verification-platform-verify-gov-kh-won-the-united-nations-public-service-award-2026/)
- [Cambodia Digital Government Policy 2022–2035 (PDF)](https://asset.cambodia.gov.kh/mptc/media/Cambodia_Digital_Government_Policy_2022_2035_English.pdf)
- [Cambodia Digital Economy and Society Policy Framework 2021–2035 (PDF)](https://asset.cambodia.gov.kh/mptc/media/EN-Policy-Framework-of-Digital-Economy-and-Society.pdf)
- [DLA Piper: Data protection laws in Cambodia](https://www.dlapiperdataprotection.com/index.html?t=law&c=KH)
