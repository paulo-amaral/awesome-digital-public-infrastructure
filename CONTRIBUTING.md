# Contributing to Awesome Digital Public Infrastructure

Thank you for helping build the most comprehensive resource on Digital Public Infrastructure (DPI) and Digital Public Goods (DPG)!

## How to Contribute

### Suggest a New Resource

1. **[Open an issue](https://github.com/paulo-amaral/awesome-digital-public-infrastructure/issues/new/choose)** using the **Add Resource** template.
2. Fill in the resource name, URL, category, and a one-sentence description.
3. A maintainer will review and merge it if it meets the criteria below.

Alternatively, you can submit a **pull request** directly (see below).

### Submit a Pull Request

1. Fork this repository.
2. Create a branch: `git checkout -b add/your-resource-name`
3. Add your resource following the [formatting rules](#formatting-rules).
4. Open a pull request with a short description of the resource and why it belongs here.

---

## Inclusion Criteria

A resource must meet **all** of the following to be included:

- **Relevant** — directly related to DPI, DPG, GovTech, digital government, or digital development.
- **Open** — software must be open source (OSI-approved license); reports/data must be openly licensed (CC BY, CC0, or similar) or freely accessible.
- **Maintained** — projects must be actively maintained (last commit or update within 2 years).
- **Not promotional** — no paid products, SaaS-only tools, or vendor marketing materials.
- **Substantive** — a brief blog post does not qualify; prefer primary sources, official docs, peer-reviewed papers, or well-cited reports.

### What Belongs Here

- Open-source platforms certified by DPGA or widely used in development contexts
- Official frameworks and standards from UN agencies, multilateral banks, or recognized standards bodies
- Country DPI profiles with documented, real-world implementations
- Assessment toolkits and procurement guidance used by practitioners
- Research papers and policy briefs from reputable institutions
- Learning resources from recognized organizations

### What Does Not Belong

- Proprietary / closed-source tools (even with a free tier)
- Unlicensed or paywalled content without a free abstract
- Personal blog posts without institutional backing
- Resources without a clear connection to DPI/DPG

---

## Formatting Rules

### General

- Each entry is one bullet point: `- [Name](URL) — One-sentence description.`
- Descriptions end with a period.
- Descriptions start with a capital letter.
- No trailing whitespace.
- Keep entries sorted **alphabetically** within each section.
- Use em dash `—` (not a hyphen `-`) to separate name from description.

### Tables (DPG Domain Section)

```markdown
| [Solution Name](https://url) | One-sentence description | License |
```

- License field: use SPDX short identifier (MIT, Apache 2.0, GPL 3.0, etc.) or `—` if not applicable.
- Keep rows sorted alphabetically by solution name within each domain table.

### Country Profiles

Country profiles live in `docs/country-profiles/`. Use the template in that directory as a starting point. Each profile should cover:

1. Overview (1 paragraph)
2. Core DPI components (table)
3. Open-source tools in use
4. Key lessons / field notes
5. References

---

## Code of Conduct

This project adheres to the [Contributor Covenant Code of Conduct](CODE_OF_CONDUCT.md). By participating, you agree to uphold it.

---

## Maintainers

This list is maintained by practitioners with field experience in digital development at UNICEF, UNDP, and partner organizations. Maintainers review pull requests within **2 weeks**.

For questions, open an issue tagged `question`.
