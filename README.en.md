# OPC Starter Skills — One-Person-Company Starter Skills (Chinese-Localized)

[![Docs](https://img.shields.io/badge/📚_docs-GitHub_Pages-42b983?style=for-the-badge)](https://kalias.github.io/OPC_starter_skills/)
[![Repo](https://img.shields.io/badge/📦_repo-kalias/OPC__starter__skills-181717?style=for-the-badge&logo=github)](https://github.com/kalias/OPC_starter_skills)
[![License](https://img.shields.io/badge/📜_license-MIT_(additions)_||_All_Rights_Reserved_(original)-blue?style=for-the-badge)](./LICENSE)

A Claude Code skills collection for indie developers / one-person-companies in the AI era, **organized in two parts**:

- **Part 1 · Mindset (The Minimalist Entrepreneur · Philosophy)** — 10 skills adapted from Sahil Lavingia's *The Minimalist Entrepreneur*. Answers "should I do this, and how do I start?"
- **Part 2 · Playbook (AI One-Person-Company · Tactics)** — 7 skills adapted from a hands-on playbook. Answers "how do I actually do it with AI?"

The two parts are **complementary, not overlapping**: Mindset covers mindset & philosophy, Playbook covers reproducible vibe-coding tactics. Use them independently, or chain them end-to-end.

> 📖 **中文版 README 请见 [/README.md](./README.md)**

---

## What it is

Two high-quality sources (*The Minimalist Entrepreneur* book + an AI one-person-company playbook) distilled into **17 invocable Claude Code skills**. Each skill is an "advisor / coach" that asks questions and renders a verdict, corresponding to one stage of the startup journey.

It's not "read the book and figure it out yourself" — it's "install it and let AI interrogate you through the framework."

## Install

### Option A: As a Claude Code plugin (recommended)

In a Claude Code session:

```
/plugin marketplace add kalias/OPC_starter_skills
/plugin install minimalist-entrepreneur
```

### Option B: Local clone

```bash
git clone git@github.com:kalias/OPC_starter_skills.git ~/.claude/plugins/opc-starter-skills
```

Then in Claude Code:

```
/plugin marketplace add ~/.claude/plugins/opc-starter-skills
/plugin install minimalist-entrepreneur
```

### Option C: Just use as prompts (no plugin install)

Each skill is just a `skills/<name>/SKILL.md` Markdown file. Feed it to any LLM and ask it to play that "advisor" — same effect.

> **Structure note**: All skills are physically flat under `skills/` (this is the Claude Code plugin loader convention — it only scans one level, `skills/<name>/SKILL.md`). The two-part split is implemented via a `part: mindset|playbook` field in frontmatter; README sections follow that split.

---

## Part 1 · Mindset (The Minimalist Entrepreneur · Philosophy)

Adapted from Sahil Lavingia's *The Minimalist Entrepreneur*. Answers "should I do this, how do I start?" The order itself is the counter-intuitive methodology — **start with community, not a product idea.**

| Skill | Command | When to use |
|-------|---------|-------------|
| **Find Community** | `/find-community` | Looking for a direction / your community |
| **Validate Idea** | `/validate-idea` | Testing whether an idea is worth pursuing |
| **MVP** | `/mvp` | Ready to build / struggling with scope |
| **Processize** | `/processize` | Want to deliver value by hand before writing code |
| **First Customers** | `/first-customers` | Have a product, need your first 100 customers |
| **Pricing** | `/pricing` | Setting prices, or considering price changes |
| **Marketing Plan** | `/marketing-plan` | Have PMF (~100 customers), ready to scale with content |
| **Grow Sustainably** | `/grow-sustainably` | Making spending / hiring / funding / scaling decisions |
| **Company Values** | `/company-values` | Defining culture, preparing to hire |
| **Minimalist Review** | `/minimalist-review` | Gut-checking any business decision |

**Core**: Don't start with "what product should I build?" — start with "whose friend am I, and what hurts for them?" You've earned the right to automate only after you've done it manually for a few people.

---

## Part 2 · Playbook (AI One-Person-Company · Tactics)

Adapted from a hands-on playbook. Answers "how do I actually do it with AI?" Core idea: **a folder is a company, skills are employees, build once and skill-ify it.**

| Skill | Command | When to use |
|-------|---------|-------------|
| **Setup AI OS** | `/setup-ai-os` | Just starting with AI indie dev, set up your company in 20 min |
| **Build Anything** | `/build-anything` | Want to build a new product, stuck on a complex project |
| **Skillify** | `/skillify` | Just finished a project, want to turn it into a reusable asset |
| **Organic Engine** | `/organic-engine` | Have product, no customers — let content pull them in |
| **Cold Outreach Engine** | `/cold-outreach-engine` | Want a "works while you sleep" lead pipeline |
| **Doctor Selling** | `/doctor-selling` | Have leads but losing deals, can't close calls |
| **Deliver and Scale** | `/deliver-and-scale` | Won a client to deliver, or want to upgrade to recurring revenue |

**Core**: A one-person-company's IP isn't code — it's SOPs / the skills folder. Anything you do twice becomes a skill.

---

## How the two parts chain together (full flow)

```
[Part 1 · Think it through]       [Part 2 · Build it with AI]
/find-community  →  /validate-idea
        │                 │
        ▼                 ▼
                    /setup-ai-os   ← set up the company
                          │
        ┌─────────────────┼─────────────────┐
        ▼                 ▼                 ▼
   /processize       /mvp              /build-anything
   (manual run)      (minimal product) (actually build it)
        │                 │                 │
        └─────────────────┼─────────────────┘
                          ▼
                     /skillify   ← turn it into a permanent asset
                          │
        ┌─────────────────┼─────────────────┐
        ▼                 ▼                 ▼
  /organic-engine  /cold-outreach    /first-customers
  (active engine)  (passive engine)  (sell manually)
        │                 │                 │
        └─────────────────┼─────────────────┘
                          ▼
                  /doctor-selling  ← close the call
                          │
                          ▼
                  /deliver-and-scale ← deliver L1/L2/L3
                          │
                          ▼
              /pricing · /marketing-plan · /grow-sustainably
              (price · scale · stay sustainable)
                          │
                          ▼
                  /minimalist-review  ← review every decision
```

---

## What the localization changed

| Category | Original | Chinese edition |
|---|---|---|
| Theoretical framework | — | 100% preserved |
| Sahil / Gumroad original cases | — | Preserved (the methodological source) |
| Tools | Stripe / Carrd / Notion / Zapier | WeChat Pay / Alipay / shangxianle / Tencent Docs / n8n, etc. |
| Platforms | Twitter / Reddit / YouTube / Substack | Xiaohongshu / Jike / V2EX / Bilibili / WeChat Official Account / zhubai |
| Examples | Nordstrom accepting tire returns | Haidilao service myth (same "story-as-value" pattern) |
| Currency | USD | CNY conversions annotated; key figures kept with original reference |
| Tone | Interrogative / pushy | Preserved (it's where the power comes from) |
| Frontmatter | English | `name` / `part` kept in English (loader depends on it), `description` translated |

---

## Suggested usage (highest ROI)

1. **You don't need all 17** — most people get stuck at `validate-idea` (should I?) and `build-anything` (how with AI?). Pick the stage you're wrestling with.
2. **Each skill forces specific answers.** Don't dodge — that's the value.
3. **The two parts are separable**: Part 1 alone for philosophy, Part 2 alone for tactics.
4. **Fork it**: just edit the Markdown. The structure is 17 `SKILL.md` files, zero code dependencies.

---

## Credits & License

**Part 1 (Mindset)** methodology and original examples belong to the original author:
- Original author: [Sahil Lavingia](https://sahillavingia.com/)
- Original repo: [slavingia/skills](https://github.com/slavingia/skills)
- Original book: [The Minimalist Entrepreneur](https://www.minimalistentrepreneur.com/)

**Part 2 (Playbook)** tactics are localized rewrites from a public hands-on playbook article.

This Chinese edition is for study and localization purposes. Full notice in [LICENSE](./LICENSE): original authors' content is All Rights Reserved; our translation and localization additions are under MIT.
