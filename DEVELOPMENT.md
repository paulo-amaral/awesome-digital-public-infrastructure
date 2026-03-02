# Development Guide

How the CI/CD works, how to submit PRs, and what good contributions look like.

---

## CI/CD — What runs automatically

Every push to `main` and every pull request triggers a link checker via GitHub Actions. It scans all links in the README, CONTRIBUTING.md, and country profiles and flags anything broken.

**Workflow file:** `.github/workflows/ci.yml`

It also runs on a weekly schedule (Mondays at 08:00 UTC) to catch links that break over time. If any links fail, it opens a GitHub issue automatically with a list of the broken URLs.

### Enabling it on a new fork

1. Go to your repository on GitHub
2. Click **Actions** tab
3. If Actions are disabled, click **"I understand my workflows, go ahead and enable them"**
4. That's it — it will run on the next push

### Running the link checker locally

Install [lychee](https://github.com/lycheeverse/lychee):

```bash
# macOS
brew install lychee

# Or with cargo
cargo install lychee
```

Then run:

```bash
lychee README.MD CONTRIBUTING.md docs/**/*.md
```

This catches broken links before you push.

---

## Branch naming

Keep it simple and consistent:

| Type | Branch name |
|------|-------------|
| Add a resource | `add/resource-name` |
| Fix a broken link | `fix/broken-link-toolname` |
| Add a country profile | `add/country-kenya` |
| Update existing content | `update/section-name` |
| CI or workflow changes | `ci/what-you-changed` |

---

## Submitting a PR

### Before you open a PR

- [ ] Run the link checker locally — no broken links
- [ ] The resource meets the criteria in [CONTRIBUTING.md](CONTRIBUTING.md)
- [ ] Descriptions are one sentence, no trailing spaces
- [ ] Entries are in alphabetical order within their section
- [ ] Country profiles use the template in `docs/country-profiles/README.md`

### PR title format

```
Add: [Resource Name]
Fix: broken link in [section]
Update: [section] — short description
Add: country profile for [Country]
```

### PR body — keep it short

```markdown
## What this adds

[Name of resource](https://url)

**Category:** Frameworks / DPGs — Health / Country Profiles / etc.

**Why it belongs here:** one or two sentences on what it is and why it's worth including.

**License:** MIT / Apache 2.0 / CC BY / etc.

**Checklist:**
- [ ] Link works
- [ ] Meets inclusion criteria
- [ ] Alphabetical order maintained
- [ ] One-sentence description
```

### After you open a PR

- The link checker runs automatically — wait for it to pass (green check)
- If it fails, look at the Actions log and fix the broken URL
- PRs are reviewed within two weeks
- Small fixes (broken links, typos) are usually merged same day

---

## Reviewing PRs

If you're reviewing someone else's contribution:

- Check the link actually works and goes where it says
- Verify the project is actively maintained (check last commit or release date)
- Make sure it's not a commercial product in disguise
- Leave a comment if you want changes — don't just close without explanation

---

## Keeping the list healthy

A few habits that help:

**When you add something**, check if something nearby is stale. If a link in the same section is broken, fix it in the same PR.

**Don't merge your own PRs** unless it's a trivial fix (broken link, typo). For anything that adds content, wait for at least one review.

**If the CI fails on `main`**, fix it before merging anything else. A broken CI is worse than no CI.

**For country profiles** — only add what you can verify. A stub profile with one real implementation detail is better than a complete-looking profile with unverified data.

---

## GitHub Actions reference

| Workflow | Trigger | What it does |
|----------|---------|-------------|
| `ci.yml` | Push to `main`, any PR, weekly on Mondays | Checks all links with lychee, opens an issue if any fail |

To trigger it manually: **Actions tab → CI — Link Checker → Run workflow**.

---

## Local setup for contributors

No build step needed — this is a Markdown list. You just need:

- A text editor
- Git
- `lychee` if you want to check links before pushing (optional but useful)

To preview the README as it will look on GitHub, use the [GitHub Markdown Preview](https://markdownlivepreview.com/) or VS Code with the built-in Markdown preview (`Cmd+Shift+V`).
