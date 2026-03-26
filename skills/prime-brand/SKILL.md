---
name: prime-brand
description: Load LowCode Agency brand context, voice guidelines, and company knowledge into the current conversation
user-invokable: true
args:
  - name: scope
    description: "What to load: voice, content, company, design, or all (default: all)"
    required: false
---

# Prime Brand

Load LowCode Agency brand context, voice guidelines, and company knowledge into the current conversation.

## Usage

```
/prime-brand
/prime-brand voice
/prime-brand content
/prime-brand company
/prime-brand design
/prime-brand all
```

## When to Use

- Before writing any content as LowCode Agency or Jesus Vargas
- Before designing or reviewing UI/UX for LowCode projects
- Before drafting proposals, emails, or client-facing materials
- When you need company context (team, pricing, services, case studies)
- Any time brand consistency matters

## Instructions

When this skill is invoked, load the relevant docs based on the argument:

### No argument or `all` — Load everything
Read all files in this order:
1. `docs/brand/brand-voice.md` — Voice identity and tone
2. `docs/brand/brand-guidelines.txt` — Visual guidelines
3. `docs/company/LOWCODE_AGENCY.md` — Company context
4. `docs/content/WRITING_GUIDELINES.md` — Writing rules
5. `docs/content/jesus-vargas-voice-profile.md` — Personal voice
6. `docs/content/content-strategy.md` — Content strategy
7. `docs/company/about-me.md` — Jesus bio
8. `docs/company/team-members.md` — Team directory
9. `docs/company/glossary.md` — Terms and acronyms
10. `docs/reference/CASE_STUDIES.md` — Case studies
11. `docs/reference/working-preferences.md` — Working preferences

### `voice` — Voice and tone only
Read:
1. `docs/brand/brand-voice.md`
2. `docs/content/jesus-vargas-voice-profile.md`
3. `docs/content/content-strategy.md` (voice reference sections)

### `content` — Content writing context
Read:
1. `docs/brand/brand-voice.md`
2. `docs/content/WRITING_GUIDELINES.md`
3. `docs/content/CONTENT_GUIDELINES.md`
4. `docs/content/CONTENT_PROMPTS.md`
5. `docs/content/jesus-vargas-voice-profile.md`
6. `docs/content/content-strategy.md`
7. `docs/reference/CASE_STUDIES.md`

### `company` — Company context
Read:
1. `docs/company/LOWCODE_AGENCY.md`
2. `docs/company/about-me.md`
3. `docs/company/team-members.md`
4. `docs/company/glossary.md`
5. `docs/reference/CASE_STUDIES.md`

### `design` — Visual and brand design context
Read:
1. `docs/brand/brand-guidelines.txt`
2. `docs/brand/brand-voice.md`

After loading, confirm what was loaded with a brief summary like:

> **Brand context loaded.** Voice, visual guidelines, and [X other docs] are now in context. Ready to work.

Do NOT summarize the contents of the docs — just confirm they're loaded and move on.
