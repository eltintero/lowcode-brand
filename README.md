# LOW / CODE Brand Kit

The single source of truth for everything about LowCode Agency — how we sound, how we look, who we are, and how we write. This repo powers Claude Code as a plugin so every AI-assisted project stays on-brand automatically.

**Stop copying `brand-guidelines.txt` into every project.** Install this once and it works everywhere.

## What's Inside

### Brand (`docs/brand/`)

| File | What it is | When to use it |
|------|-----------|----------------|
| **brand-voice.md** | Voice identity, tone rules, writing do's/don'ts, positioning | Writing anything as LowCode Agency — website copy, proposals, emails, social |
| **brand-guidelines.txt** | Visual system — logo, colors, typography, layout rules, what to avoid | Designing UI, reviewing mockups, building presentations, creating assets |

### Company (`docs/company/`)

| File | What it is | When to use it |
|------|-----------|----------------|
| **LOWCODE_AGENCY.md** | Master company prompt — history, services, pricing, clients, team structure, USPs | Proposals, sales decks, client-facing materials, onboarding new team members |
| **about-me.md** | Jesus Vargas bio — background story, values, online presence, leadership style | Content written as Jesus, press kits, speaker bios, about pages |
| **team-members.md** | Full team directory — 40 people, roles, department structure | Internal reference, project assignments, org context |
| **glossary.md** | Internal terms, acronyms, platform names, pricing shorthand | When you need to know what "AEO", "PE", "3-Tier Proposal", or "$15K project" means |

### Content (`docs/content/`)

| File | What it is | When to use it |
|------|-----------|----------------|
| **WRITING_GUIDELINES.md** | Full writing rulebook — AEO optimization, article structure, header formatting, answer boxes, FAQ format, quality checklist | Writing any blog post, landing page, or SEO content |
| **CONTENT_GUIDELINES.md** | Blog-specific guidelines for the SEO team — tone, structure, keyword rules, intro/conclusion format | Blog posts and SEO articles specifically |
| **CONTENT_PROMPTS.md** | Prompts for outline creation and article generation | Starting a new blog post from a keyword |
| **content-strategy.md** | Platform strategy (LinkedIn, Twitter, YouTube, Newsletter), topical pillars, voice by channel, content pipeline | Planning content, choosing the right tone for each platform |
| **jesus-vargas-voice-profile.md** | Deep personal voice profile — rhetorical habits, tone spectrum, personality traits, formatting DNA | Writing anything in Jesus's voice — newsletters, LinkedIn, Twitter, YouTube scripts |

### Reference (`docs/reference/`)

| File | What it is | When to use it |
|------|-----------|----------------|
| **CASE_STUDIES.md** | All case studies organized by platform (Glide, Bubble, FlutterFlow, Webflow) with metrics and links | Proposals, blog posts, social proof, sales conversations |
| **portfolio-highlights.md** | Curated portfolio showcase — tiered by impact, with metrics, quotes, timelines, and a "best project by use case" matching guide | Sales decks, proposals, social proof, picking the right case study for a prospect |
| **working-preferences.md** | How Jesus wants AI tools to communicate and work with him | AI/Claude configuration — communication style, output format, priorities |

## Quick Reference

| | |
|---|---|
| **Logo** | LOW / CODE (forward slash always present) |
| **Primary palette** | Purple (#705CF6), Dark purple (#38327C), Cream (#FAF9F6) |
| **Accent** | Lime (#C5EF48) — sparingly, dark contexts only |
| **Typography** | Inter (Bold titles, Regular body, Semi Bold buttons) |
| **Tagline** | "Fast isn't enough. We build forward, think strategically, and run as a product team." |
| **Key stats** | 40 team / 350+ projects / 7-figure revenue / Sotheby's, AMEX, Coca-Cola, Zapier |

## Setup (Claude Code Plugin)

Two commands. Takes 30 seconds.

```bash
# 1. Clone the repo
git clone https://github.com/eltintero/lowcode-brand.git ~/projects/lowcode-brand

# 2. Symlink into Claude Code plugins
ln -s ~/projects/lowcode-brand ~/.claude/plugins/lowcode-brand
```

Done. Claude Code will:
- Auto-load the brand quick reference into every conversation (via CLAUDE.md)
- Make `/prime-brand` available as a skill in every project

### Updating

```bash
cd ~/projects/lowcode-brand && git pull
```

Changes propagate instantly to all projects. No more copy-pasting files.

## Using `/prime-brand`

Load brand context into your current Claude Code session:

```
/prime-brand          # Load everything
/prime-brand voice    # Voice and tone guidelines only
/prime-brand content  # Writing rules, SEO guidelines, voice profile, case studies
/prime-brand design   # Visual guidelines — colors, typography, layout
/prime-brand company  # Company info, team directory, pricing, case studies
```

**Use it before:**
- Writing content (blog, social, newsletter, proposals)
- Designing or reviewing UI
- Drafting client-facing materials
- Anything where brand consistency matters

## How to Edit

This repo is the canonical source. To update any brand doc:

1. Edit the file in `docs/`
2. Commit and push
3. Everyone gets the update on next `git pull`

**Do not** copy these files into other project repos. Reference this repo instead.

## Repo Structure

```
lowcode-brand/
├── CLAUDE.md                              # Quick reference (auto-loaded by Claude Code)
├── docs/
│   ├── brand/
│   │   ├── brand-voice.md                 # Voice identity, tone, writing rules
│   │   └── brand-guidelines.txt           # Visual: logo, colors, typography, layout
│   ├── company/
│   │   ├── LOWCODE_AGENCY.md              # Master company prompt
│   │   ├── about-me.md                    # Jesus Vargas bio
│   │   ├── team-members.md                # Full team directory
│   │   └── glossary.md                    # Internal terms and acronyms
│   ├── content/
│   │   ├── WRITING_GUIDELINES.md          # Full writing rules (AEO, structure)
│   │   ├── CONTENT_GUIDELINES.md          # Blog-specific guidelines (SEO team)
│   │   ├── CONTENT_PROMPTS.md             # Outline and article generation prompts
│   │   ├── content-strategy.md            # Platforms, pillars, voice by channel
│   │   └── jesus-vargas-voice-profile.md  # Personal voice profile
│   └── reference/
│       ├── CASE_STUDIES.md                # All case studies by platform
│       ├── portfolio-highlights.md        # Tiered portfolio showcase with metrics and quotes
│       └── working-preferences.md         # AI working preferences
└── skills/
    └── prime-brand/
        └── SKILL.md                       # /prime-brand skill definition
```
