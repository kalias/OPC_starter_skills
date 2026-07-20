# The Minimalist Entrepreneur — Claude Code Skills (Chinese-Localized Edition)

A Chinese-localized set of Claude Code skills based on
[*The Minimalist Entrepreneur*](https://www.minimalistentrepreneur.com/)
by Sahil Lavingia.

> **Original project**: [slavingia/skills](https://github.com/slavingia/skills) (English)
> **Author background**: Sahil Lavingia dropped out of USC at 17 to become
> Pinterest's first designer, then built Gumroad in a weekend at 19. The book
> codifies his "community-first, validate-first, manual-first, charge-from-day-one"
> approach to building a minimalist business.
> **This repo**: Faithfully preserves the original book's framework and Sahil's
> Gumroad case studies. Tools, platforms, channels, and examples are adapted
> for the Chinese market.

> 📖 **中文版 README 请见 [/README.md](./README.md)**

---

## What it is

[*The Minimalist Entrepreneur*](https://www.minimalistentrepreneur.com/) distilled
into **10 invocable Claude Code skills**. Each skill is an "advisor" that asks
questions and renders a verdict, corresponding to one stage of the book's
entrepreneurship journey.

It's not "read the book and figure it out yourself" — it's "install it and let
AI interrogate you through the book's framework."

## Install

### Option A: As a Claude Code plugin (recommended)

In a Claude Code session:

```
/plugin marketplace add kalias/OPC_starter_skills
/plugin install minimalist-entrepreneur
```

### Option B: Local clone

```bash
git clone git@github.com:kalias/OPC_starter_skills.git ~/.claude/plugins/zai-skills-zh
```

Then in Claude Code:

```
/plugin marketplace add ~/.claude/plugins/zai-skills-zh
/plugin install minimalist-entrepreneur
```

### Option C: Just use as prompts (no plugin install)

Each skill is just a `skills/<name>/SKILL.md` Markdown file. Feed it to any LLM
(Claude, ChatGPT, etc.) and ask it to play that "advisor" — the effect is the
same.

---

## The 10 skills

| Skill | Command (CN) | When to use |
|-------|---------|-------------|
| **找社区** (Find Community) | `/find-community` | Looking for a direction / your community |
| **验证想法** (Validate Idea) | `/validate-idea` | Testing whether an idea is worth pursuing |
| **MVP** | `/mvp` | Ready to build / struggling with scope |
| **流程化** (Processize) | `/processize` | Want to deliver value by hand before writing code |
| **前 100 个客户** (First Customers) | `/first-customers` | Have a product, need your first 100 customers |
| **定价** (Pricing) | `/pricing` | Setting prices, or considering price changes |
| **营销方案** (Marketing Plan) | `/marketing-plan` | Have PMF (~100 customers), ready to scale with content |
| **可持续增长** (Grow Sustainably) | `/grow-sustainably` | Making spending / hiring / funding / scaling decisions |
| **公司价值观** (Company Values) | `/company-values` | Defining culture, preparing to hire |
| **极简复盘** (Minimalist Review) | `/minimalist-review` | Gut-checking any business decision |

---

## The Minimalist Entrepreneur journey

The skill order *is* the methodology — and it runs **against** most people's
intuition of "idea → build product → find customers":

1. **Community** — Start by finding your people
2. **Validate** — Make sure the problem is worth solving
3. **Build** — Ship a manual process, then productize it
4. **Processize** — Turn your product idea into a manual process you can deliver today
5. **Sell** — Get to 100 customers one by one
6. **Price** — Charge something from day one
7. **Market** — Build an audience through content
8. **Grow** — Stay profitable, grow sustainably
9. **Culture** — Build the house you want to live in
10. **Review** — Apply minimalist principles to every decision

**Counter-intuitive core**: Don't start with "what product should I build?" —
start with "whose friend am I, and what hurts for them?" You've earned the right
to automate only after you've done it manually for a few people.

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
| Frontmatter | English | `name` kept in English (plugin loader depends on it), `description` translated |

---

## Suggested usage (highest ROI)

1. **You don't need all 10** — most people get stuck at `validate-idea` and
   `pricing`. Pick the stage you're wrestling with.
2. **Each skill forces specific answers** ("Can you name 10 specific people who
   have this problem?"). Don't dodge — that's the value.
3. **Fork it**: just edit the Markdown. The structure is 10 `SKILL.md` files,
   zero code dependencies.

---

## Credits

- Original author: [Sahil Lavingia](https://sahillavingia.com/)
- Original repo: [slavingia/skills](https://github.com/slavingia/skills)
- Original book: [The Minimalist Entrepreneur](https://www.minimalistentrepreneur.com/)

This Chinese edition is for study and localization purposes. Copyright of the
methodology and original examples belongs to Sahil Lavingia. See [LICENSE](./LICENSE)
for the full notice.
