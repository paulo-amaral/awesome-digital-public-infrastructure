# India — DPI Profile

## Overview

India has built one of the world's most comprehensive Digital Public Infrastructure stacks — commonly known as **India Stack** — over the past decade. The stack is built on three foundational layers: identity (Aadhaar), consent-based data sharing (Account Aggregator), and payments (UPI). Together they serve 1.4 billion people and have become a reference model studied by governments globally.

India's approach is notable for its **population-scale design**: each layer was built to handle hundreds of millions of transactions per day from inception, using open APIs and open standards that any private or public actor can build upon.

## DPI Stack

| Layer | Solution | Launch | Scale |
|-------|----------|--------|-------|
| Foundational ID | [Aadhaar](https://uidai.gov.in/) | 2009 | 1.38B enrollments |
| Digital Identity Auth | [DigiLocker](https://www.digilocker.gov.in/) | 2015 | 300M+ users |
| Instant Payments | [UPI](https://www.npci.org.in/what-we-do/upi/product-overview) | 2016 | 14B+ txn/month |
| Open Commerce | [ONDC](https://ondc.org/) | 2022 | Growing |
| Health ID | [Ayushman Bharat ABDM](https://abdm.gov.in/) | 2021 | 500M+ records |
| Consent Layer | [Account Aggregator](https://sahamati.org.in/) | 2021 | Live |
| Agriculture Data | [AgriStack](https://agriwelfare.gov.in/) | 2023 | Rollout |

## Open-Source Tools and Specifications

- [UPI Specification](https://www.npci.org.in/) — Open API specifications for interoperable payments
- [ABDM Health Data Management Policy](https://abdm.gov.in/) — Open standards for health data exchange
- [Sunbird](https://sunbird.org/) — Open-source DPI for education (powers DIKSHA, used by 70M+ students)
- [MOSIP](https://mosip.io/) — Foundational ID platform open-sourced from India's experience

## Key Milestones

- **2009:** Aadhaar program launched by UIDAI
- **2016:** UPI goes live — real-time, interoperable payments via mobile
- **2020:** India Stack API opens to global developers
- **2021:** Account Aggregator framework enables consent-based data sharing
- **2022:** ONDC launches open network for e-commerce
- **2023:** India presents India Stack at G20 as a model for global DPI adoption

## Lessons Learned

- **Open APIs multiply impact:** Making each layer freely accessible via open APIs enabled thousands of private-sector applications to build on public infrastructure.
- **Identity as a platform, not a card:** Aadhaar's value is not the ID card but the authentication API — enabling remote, paperless verification at scale.
- **Interoperability over consolidation:** UPI's success came from mandating interoperability between banks rather than building a single government payment app.
- **Trust requires governance:** Strong data protection frameworks and opt-out mechanisms are essential for public adoption of identity systems at scale.
- **Sequencing matters:** Identity → Payments → Data Exchange is the proven sequence. Each layer enables the next.

## References

- [India Stack — Official](https://www.indiastack.org/)
- [iSPIRT: The Story of India Stack](https://ispirt.in/)
- [Co-Develop: India's DPI Journey](https://www.co-develop.net/)
- [G20 DPI Report 2023](https://www.g20.org/)
- [World Bank: Digital India Assessment](https://www.worldbank.org/en/country/india/publication/digital-india)
