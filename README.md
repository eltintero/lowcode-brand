# lowcode-brand

Single source of truth for LowCode Agency's brand identity, voice, writing guidelines, and company context.

## What's in here

- **Brand voice & visual guidelines** — How we sound and look
- **Writing guidelines** — AEO-optimized content structure, SEO rules, formatting
- **Voice profile** — Jesus Vargas's personal writing voice
- **Company context** — Team, services, pricing, case studies, glossary
- **Content strategy** — Platforms, pillars, voice by channel

## Setup for Claude Code

Add this repo as a plugin so every project gets access to the brand context:

### Option 1: Global plugin (recommended)

Add to `~/.claude/settings.json`:

```json
{
  "plugins": [
    "/path/to/lowcode-brand"
  ]
}
```

### Option 2: Per-project plugin

Add to your project's `.claude/settings.json`:

```json
{
  "plugins": [
    "/path/to/lowcode-brand"
  ]
}
```

### Option 3: Symlink into any project

```bash
ln -s /path/to/lowcode-brand/.claude/plugins/lowcode-brand your-project/.claude/plugins/lowcode-brand
```

## Usage

Once installed, use the skill:

```
/prime-brand          # Load all brand context
/prime-brand voice    # Voice and tone only
/prime-brand content  # Content writing context
/prime-brand design   # Visual brand guidelines
/prime-brand company  # Company info, team, case studies
```

The CLAUDE.md at the root also provides a quick-reference summary that's always loaded.

## Updating

This is the canonical source. Edit docs here, commit, and push. All projects using this as a plugin will pick up changes automatically (no copy-paste needed).

## Structure

```
lowcode-brand/
├── CLAUDE.md                              # Hot cache / quick reference (always loaded)
├── docs/
│   ├── brand/
│   │   ├── brand-voice.md                 # Voice identity, tone, writing rules
│   │   └── brand-guidelines.txt           # Visual: logo, colors, typography, layout
│   ├── company/
│   │   ├── LOWCODE_AGENCY.md              # Master company prompt
│   │   ├── about-me.md                    # Jesus Vargas bio
│   │   ├── team-members.md                # Full team directory
│   │   └── glossary.md                    # Internal terms
│   ├── content/
│   │   ├── WRITING_GUIDELINES.md          # Full writing rules (AEO, structure)
│   │   ├── CONTENT_GUIDELINES.md          # Blog-specific guidelines
│   │   ├── CONTENT_PROMPTS.md             # Outline & article generation prompts
│   │   ├── content-strategy.md            # Platforms, pillars, voice by channel
│   │   └── jesus-vargas-voice-profile.md  # Personal voice profile
│   └── reference/
│       ├── CASE_STUDIES.md                # All case studies by platform
│       └── working-preferences.md         # How Jesus wants AI to work
└── skills/
    └── prime-brand/
        └── SKILL.md                       # /prime-brand skill definition
```
