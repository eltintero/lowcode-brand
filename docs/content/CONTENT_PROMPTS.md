# Content Generation Prompts

## Outline Creation Process

*(Use this only when input is "Keyword" and not an outline.)*

### Step 1

I want to rank in the top 3 for the keyword "{Keyword}".

Scan the entire SERP and analyze the top 10 ranking pages.

Give me a complete list of all the topics, subtopics, and key points they cover.

Do not write an outline or explanations - only provide a bullet-point list of every point they include, merged and deduplicated.

### Step 2

From the above points, give me only the points that match the real user intent behind the keyword "{Keyword}".

First, identify what the user's intent and expectations are when they search this keyword.

Then filter the point list so only intent-relevant points remain.

After that, add all missing but necessary points that top competitors are *not* covering but are essential to fully satisfy user intent, increase topical depth, and help the article rank in the top 3.

Do not write explanations - only provide a clean combined point list.

### Step 3

Arrange all these points in the correct logical order.

Your job is to help me create the best outline for the writer.

Give the outline in proper H1, H2, H3, and bullet point format.

Make sure the structure flows logically from beginner context to advanced execution.

Keep headings clean, short, and organized.

Do NOT merge, change, or remove any topics given below.

Only rearrange the order if needed for a better reading journey.

Also follow these guidelines:

- Use H1 for the title, H2 for the main sections, and H3 for sub-sections.
- Place bullet points under each H3 if additional context is provided.
- If the topic represents a process, organize steps in the natural workflow order.
- Ensure the outline reflects teaching progression: Introduction -> Definition -> Planning -> Building -> Testing -> Iteration -> Future -> Conclusion -> FAQs
- Make the outline easy for writers to follow and expand into full articles.
- Add short 1-line summary below each H2 to explain what the section covers (not content, just context).
- Do not write content, only structure.

---

## Article Creation Prompt

*(Use this when input is "Outline" and not a keyword.)*

I'm writing an article on "{Keyword}", and I need your help.

I will give you an outline, and you must write the best possible content for each section.

Follow all the instructions in docs/content/WRITING_GUIDELINES.md strictly.

Also, check the docs/content/WRITING_GUIDELINES.md and docs/reference/CASE_STUDIES.md try inserting about "LowCode Agency" wherever possible in the relevant sections.

Use a 9th-grade reading level and an A2 English level.

Keep the content factual, unique, and plagiarism-free.

Write in the voice of an expert no-code / low-code developer, automation specialist, founder, and AI expert.

Make the content clear, helpful, and accurate.

Here is the {Outline}
