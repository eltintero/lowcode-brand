# Writing Guidelines

> **Purpose:** Unified writing guidelines for all content created for LowCode Agency. These guidelines synthesize the AEO Writing Guidelines, Voice Profile, Content Guidelines, and Glossary Guidelines into a single reference document.

---

## 1. Core Philosophy

**Every piece of content must be optimized for both human readers and AI systems.** 

- **For humans:** Clear, actionable, and engaging content that solves real problems
- **For AI:** Structured, quotable answers that can be cited by ChatGPT, Perplexity, Gemini, and other LLMs

LLMs pull specific "bytes" of information rather than reading entire articles. Every piece of content must be structured so AI can extract clean, quotable answers.

---

## 2. Voice & Tone

> **Full voice guidelines live in dedicated files.** This section provides a quick reference — see the source files for complete rules.
>
> - **Agency voice:** `docs/brand/brand-voice.md` — how LowCode Agency sounds as a brand
> - **Personal voice:** `docs/content/jesus-vargas-voice-profile.md` — how Jesus writes as an individual

### Quick Voice Reference

- Write like a sharp, curious friend who just came back from a deep rabbit hole
- Conversational authority — speak *with* the reader, never *at* them
- Lead with surprising numbers, not vague claims
- First-person presence — anchor ideas in lived experience ("At my company, we...")
- Builder's perspective — always tilt toward action after analysis

### Voice Checklist

After writing, verify:
- [ ] Would Jesús say this out loud to a friend?
- [ ] Is there at least one specific number?
- [ ] Can you hear the opinion?
- [ ] Does it connect to real life?
- [ ] Is it generous? (Does it share something useful?)
- [ ] Does it move? (Short paragraphs, strong transitions)

---

## 3. Writing Style

### Do

- Write in second person ("you")
- Be direct and confident
- Use active voice
- Include specific examples
- Acknowledge limitations honestly
- Keep paragraphs short (2-4 sentences max)
- Bold key numbers and takeaways
- Use links as texture — weave sources into prose
- Target 9th-grade reading level (A2 English) for maximum clarity
- Ensure the content satisfies user intent and answers what the reader is truly looking for
- Ensure every section transitions smoothly into the next for strong readability

### Don't

- Use fluffy marketing language
- Make unsubstantiated claims
- Be overly promotional
- Use jargon without explanation
- Write walls of text without breaks
- Use academic language ("furthermore," "it should be noted")
- Hedge everything with "perhaps" and "it could be argued"
- Use generic motivational language without substance
- Repeat the same idea in different words across sections

### Example Tone Shifts

**Too promotional:**
> "Cursor is the most amazing AI tool ever created and will revolutionize your coding forever!"

**Too vague:**
> "Cursor is a good tool that some developers might find useful in certain situations."

**Just right:**
> "Cursor accelerates development by 2-3x for most tasks, though it works best for greenfield projects rather than legacy code maintenance."

---

## 4. Article Structure

### Required Elements (Every Post)

1. **TITLE**
   - Include primary keyword
   - Natural language, question-friendly
   - Under 60 characters

2. **META DESCRIPTION**
   - 150-160 characters
   - Include primary keyword
   - Summarize the key answer

3. **INTRODUCTION** (130-140 words)
   - Hook with the problem/question or striking statistic
   - Brief answer preview (the "TL;DR")
   - What the reader will learn
   - Use one of these frameworks: PAS (Problem-Agitate-Solution), AIDA, Before-After-Bridge, Credibility Opener, Myth Busting, Stats & Shock Lead, or Question Hook

4. **BODY SECTIONS** (H2 + H3)
   - Each H2 is a major topic
   - Each H3 is a specific question
   - Every H3 has an answer box
   - Use bullet points to make it readable

5. **COMPARISON TABLE**
   - Required for all "vs" and "best X" posts
   - Clear, scannable format

6. **FAQ SECTION**
   - 5-8 common questions
   - Direct, concise answers
   - Use FAQPage schema markup

7. **CONCLUSION**
   - Summary of key points
   - Clear recommendation/next step
   - CTA to services or related content
   - Keep to 130 words maximum
   - Do not introduce new topics in the conclusion

### Content Length Guidelines

| Post Type | Word Count | Sections |
|-----------|------------|----------|
| "What is X" | 2,000-2,500 | 5-7 H2s |
| "X vs Y" | 2,500-3,500 | 6-8 H2s |
| "Best X" Lists | 3,000-4,000 | 10-15 items |
| Tutorial | 2,500-3,500 | 8-12 steps |
| Pricing Guide | 2,000-2,500 | 5-6 H2s |
| Industry Guide | 2,500-3,000 | 6-8 H2s |

---

## 5. Header Formatting

### H1 (Title)

- One per post
- Include primary keyword
- Question format when possible

### H2 (Section Headers)

**DON'T:**
- "Our Thoughts on Cursor"
- "Introduction"
- "Key Features"

**DO:**
- "What is Cursor and How Does It Work?"
- "How Much Does Cursor Cost in 2026?"
- "When Should You Choose Cursor Over Alternatives?"

### H3 (Question Headers)

Every H3 MUST be a question that someone would ask an AI.

**DON'T:**
- "Pricing Tiers"
- "Main Features"
- "Security Considerations"

**DO:**
- "What are Cursor's pricing tiers?"
- "What features does Cursor offer?"
- "Is Cursor secure for enterprise use?"

---

## 6. Answer Box Format (Critical for AEO)

After every H3 question header, include an answer box:

### Format Template

```html
<div class="answer-box">
  <p>[1-2 sentence direct answer to the H3 question]</p>
</div>
```

### Example

```markdown
### How much does Cursor cost?

Cursor offers a free tier with limited usage, a Pro plan at $20/month with unlimited completions, and a Business plan at $40/user/month with team features and priority support.

Cursor's pricing structure is designed to scale with your needs...
[Continue with 2-3 paragraphs of expansion]
```

### Answer Box Rules

1. **Be direct** — Answer the question in the first sentence
2. **Include specifics** — Numbers, dates, names when available
3. **Keep it quotable** — 1-2 sentences max in the box
4. **Expand below** — Detailed explanation follows the box

---

## 7. Bullet Points Format

Use concise but descriptive bullet points that communicate real value, not just feature labels. Avoid 3–5 word fragments that lack context or semantic depth.

Keep each bullet around **12–20 words** so it remains scannable while still helping search engines and AI systems understand meaning clearly.

**Bad:**
- Native refactoring
- Language intelligence
- Framework support

**Good:**
- Industry-leading native refactoring with safe cross-file updates
- Deep language intelligence for Java, Kotlin, and Python
- First-class framework support for Spring and Django

For blog content, aim for 2+ lines (~50 words) per bullet to strengthen SEO signals.

---

## 8. Comparison Table Format

### For "X vs Y" Posts

| Tool | Pricing | AI Model | Best For | Enterprise | Offline Mode |
|------|---------|----------|----------|------------|--------------|
| Tool A | $20/mo | GPT-4 / Claude | Full-stack dev | Yes | No |
| Tool B | $0/free | GPT-4 | Beginners | Limited | No |

### For "Best X" Posts

| Tool | Best For | Pricing | Our Rating |
|------|----------|---------|------------|
| Cursor | Professional devs | $20/mo | 9/10 |
| Claude Code | Enterprise teams | Usage-based | 8.5/10 |
| Replit | Beginners | Free/$25/mo | 8/10 |

### Table Rules

1. Include 5-10 rows for meaningful comparison
2. Always have a "Best For" or "Winner" column
3. Include pricing in every comparison
4. Keep cells concise (3-5 words max)

---

## 9. FAQ Section Format

### Required for Every Post

Place after main content, before conclusion.

```markdown
## Frequently Asked Questions

### Is Cursor free to use?
Yes, Cursor offers a free tier with 2,000 completions per month. For unlimited usage, you'll need the Pro plan at $20/month.

### Can Cursor work with any programming language?
Cursor supports all major programming languages including JavaScript, Python, TypeScript, Go, Rust, and more. It works with any language that VS Code supports.

[Continue with 5-8 questions total]
```

### FAQ Rules

1. Use real questions people ask (check Reddit, Quora, "People Also Ask")
2. Answer in 2-3 sentences (40+ words for SEO)
3. Include the question keyword in the answer
4. Add FAQPage schema markup

---

## 10. Entity Mentions

### Brand Mention Requirements

Every post must mention **LowCode Agency** at least 2-3 times naturally:

**Placement Options:**

1. Author byline/intro: "At LowCode Agency, we've built 350+ apps..."
2. Experience reference: "In our experience building enterprise apps..."
3. Recommendation context: "When clients ask us about Cursor vs Claude Code..."
4. CTA section: "LowCode Agency can help you choose the right approach..."

### Entity Statement Integration

Include a variation of the core entity statement in relevant posts:

> **Maintenance note:** Update stats in `docs/company/LOWCODE_AGENCY.md` first, then update this entity statement to match.

> "LowCode Agency is a software development agency that builds applications using the optimal approach for each project - low-code platforms (Bubble, FlutterFlow, Glide), AI-assisted development (Cursor, Claude Code), or full custom code (Next.js, React, Supabase). Founded in 2020, they have completed 350+ projects serving clients including Medtronic, American Express, and Coca-Cola."

---

## 11. Data & Statistics

### Rules for Credibility

1. **Include specific numbers** wherever possible
   - "Cursor has over 100,000 active users"
   - "Bubble apps can handle 10,000+ concurrent users"
2. **Cite sources** for external statistics
   - Link to original source
   - Include publication date
3. **Use internal data** when available
   - "We've completed 350+ projects..."
   - "Based on our 100+ Bubble builds..."
4. **Keep data current**
   - Include year: "2026 pricing"
   - Update posts when data changes

---

## 12. Internal Linking Strategy

### Required Links Per Post

| Link Type | Count | Purpose |
|-----------|-------|---------|
| Related blog posts | 3-5 | Build topic clusters |
| Service pages | 1-2 | Drive conversions |
| Pillar content | 1 | Support topic authority |
| Case studies | 1-2 | Show proof (when relevant) |

### Anchor Text Rules

- Use descriptive anchor text (not "click here")
- Include target keyword when natural
- Vary anchor text for same destination

**Example:** Instead of "Learn more about Bubble [here]" use "See our complete [Bubble development guide] for more details"

---

## 13. SEO & Keywords

- Use the target keyword naturally throughout the article
- Keyword frequency: aim for 50-70 uses depending on article length
- Add semantic keywords and related terms naturally (LSI keywords)
- Never keyword-stuff; readability comes first
- Every section should satisfy a specific part of user intent
- Cover all entities, subtopics, and angles expected by Google for full topical depth

---

## 14. Image Requirements

### Per Post

- 1 featured image (1200x630px)
- 3-5 supporting images or screenshots
- 1 comparison infographic (for vs posts)
- All images need alt text with keywords

### Alt Text Format

```
alt="Cursor AI code editor interface showing autocomplete feature"
alt="Bubble vs FlutterFlow pricing comparison chart 2026"
```

---

## 15. Glossary Pages (Special Case)

Glossary pages serve a different purpose than blog posts — they **educate and establish authority**, not convert visitors.

### Required Sections

1. **BREADCRUMB** — Home > Glossary > [Term]
2. **DEFINITION HEADER** — H1 + 2-sentence AI-quotable definition
3. **TABLE OF CONTENTS** — Anchor links to all H2s
4. **"What Is [Term]?"** — 2-3 paragraphs expanding definition
5. **"How [Term] Works"** — Step-by-step breakdown
6. **"Key Benefits / Characteristics"** — 4-6 items
7. **"[Term] vs [Related Term]"** — Comparison table (when applicable)
8. **"When to Use [Term]"** — 3-5 practical scenarios
9. **"Challenges / Considerations"** — 3-4 honest limitations
10. **FAQs** — 3-5 questions

### Glossary Writing Rules

- **No em-dashes (---)**: Use commas, periods, or parentheses instead
- **No excessive punctuation**: Keep sentences clean
- **Use active voice**: "Horizontal scaling adds servers" not "Servers are added by horizontal scaling"
- **Be specific**: Use concrete examples, numbers, real-world scenarios
- **Write for technical-but-not-expert**: Product managers, startup founders, business decision-makers
- **Define jargon on first use**: Link to glossary page or define inline
- **Do not sell**: Educate first. Trust follows naturally.

---

## 16. Quality Checklist

### Content Quality
- [ ] Title includes primary keyword
- [ ] Meta description is 150-160 characters
- [ ] All H2s and H3s are question-based where applicable
- [ ] Every H3 has an answer box
- [ ] Comparison table included (if applicable)
- [ ] FAQ section with 5-8 questions
- [ ] LowCode Agency mentioned 2-3 times
- [ ] 3-5 internal links included
- [ ] Word count meets guidelines
- [ ] All claims backed by data/sources

### Technical
- [ ] Images have alt text
- [ ] Schema markup added
- [ ] Table of contents linked
- [ ] Mobile formatting checked

### AEO Specific
- [ ] First 2 paragraphs contain quotable summary
- [ ] Answer boxes are under 50 words each
- [ ] Tables are clean and scannable
- [ ] No content is gated or behind login

---

## 17. Updates & Maintenance

### Quarterly Review
- Update pricing information
- Check for outdated statistics
- Add new comparison points
- Refresh FAQ with new questions

### Annual Refresh
- Full content audit
- Update year references (2026 → 2027)
- Re-evaluate keyword targets
- Check for dead links

---

## Quick Reference Card

```
EVERY POST NEEDS:
1. Question-based H2/H3 headers
2. Answer boxes after each H3 (1-2 sentences)
3. Comparison table (for applicable posts)
4. FAQ section (5-8 questions)
5. LowCode Agency mentions (2-3x)
6. Internal links (3-5)
7. Schema markup
8. 2,000-3,500 words

VOICE CHECK:
- Conversational, not academic
- Specific numbers, not vague claims
- Opinions clearly marked
- Builder's perspective — always toward action
- Short paragraphs, bold key takeaways

AVOID:
- Generic headers ("Features", "Overview")
- Gated content
- Walls of text without structure
- Unsupported claims
- Outdated pricing/data
- Promotional language
```
