# Security

This repository is a curated Markdown list. There is no application code, no database, and no user data processed here. That said, the attack surface is not zero — a list of URLs and GitHub Actions workflows carries its own risks, and contributors should understand them.

---

## For Contributors

### 1. Submitting URLs

Every link you submit will be reviewed before merging. Before opening a PR, verify the following yourself:

- **The URL resolves to what you say it does.** Visit it. Don't submit URLs you haven't personally reviewed.
- **The domain is authoritative.** Official project sites, government portals, UN agency pages, and established research institutions. Avoid personal blogs, mirror sites, or third-party aggregators unless there is a clear reason.
- **Check for typosquatting.** A domain like `govstack.io` vs `govstack.global` — one is the real project, the other might not be. Always confirm the canonical domain from the official GitHub org or Wikipedia.
- **No redirect chains to unknown destinations.** URL shorteners (bit.ly, tinyurl) are not accepted. Use the final destination URL.
- **CC, CC0, or open license only.** Paywalled content, login-gated resources, and proprietary reports do not belong here unless there is a free version.

### 2. GitHub Actions

If you contribute to the CI/CD workflow (`.github/workflows/`):

- **Pin all third-party actions to a full commit SHA**, not a tag or branch name. Tags can be moved; SHAs cannot.
  ```yaml
  # Good
  uses: actions/checkout@11bd71901bbe5b1630ceea73d27597364c9af683  # v4.2.2

  # Bad
  uses: actions/checkout@v4
  uses: actions/checkout@main
  ```
- **Request only the permissions you need.** The default permission for this repo is `contents: read`. Do not request `write` unless you can justify it in the PR description.
- **Never echo secrets.** Even indirect logging of `${{ secrets.GITHUB_TOKEN }}` or other secrets will result in the PR being closed.
- **Scope permissions at the job level**, not at the workflow level. Prefer:
  ```yaml
  jobs:
    my-job:
      permissions:
        contents: read
  ```
  over a broad top-level `permissions` block that applies to all jobs.

### 3. Dependabot

Dependabot is configured to open weekly PRs for GitHub Actions updates. When reviewing those PRs:

- Check the SHA being updated to — follow the link to the action's release page and confirm it corresponds to the expected version.
- Major version bumps (e.g. v3 → v4) require manual review before merging. Dependabot is configured to skip them automatically, but double-check.

---

## Reporting a Security Issue

If you find something that should not be in this list — a link that redirects to harmful content, a compromised domain, or a workflow change that looks suspicious — please report it privately rather than opening a public issue.

**Email:** paulo.security@gmail.com
**Subject:** `[SECURITY] awesome-digital-public-infrastructure`

Include:
- What you found
- The URL, file, or workflow step involved
- Steps to reproduce if applicable

You will receive a response within 72 hours.

---

## What Can Go Wrong — Threat Model

| Risk | How it happens | Mitigation |
|------|---------------|-----------|
| Malicious link | Contributor submits a URL that later redirects to phishing or malware | Manual review before merge; automated link checks on every PR |
| Typosquatting | URL resembles a known DPG project but points elsewhere | Reviewer checks domain ownership; lychee checks that it resolves |
| Compromised GitHub Action | A pinned action's underlying commit is replaced (extremely rare but possible) | SHA pinning + Dependabot alerts if a new version is available |
| Overpermissioned workflow | A workflow requests write access it does not need | `permissions: contents: read` is the default; job-level scoping enforced |
| Supply chain via fork | A fork of a dependency action is substituted | All actions must come from verified namespaces (github, actions, lycheeverse, peter-evans) |

---

## Hardening in Place

| Control | Status |
|---------|--------|
| GitHub Actions pinned to SHA | Active |
| Minimal workflow permissions (`contents: read` default) | Active |
| Automated link checking on every PR (lychee) | Active |
| `.lycheeignore` for rate-limited domains | Active |
| Dependabot for Actions updates | Active |
| CODEOWNERS — all changes reviewed by maintainer | Active |
| Branch protection — require PR + status checks on `main` | Recommended (set manually in Settings → Branches) |

---

## Supported Versions

Only the current `main` branch is maintained. There are no versioned releases that receive security backports.

---

*Maintained by [@paulo-amaral](https://github.com/paulo-amaral). Security recommendations follow NIST SP 800-53, CIS Controls, and GitHub's own hardening guidance for public repositories.*
