---
name: removeai-academic
description: Humanize Chinese academic writing, research collaboration text, essays, reports, proposals, literary essays, social posts, Xiaohongshu-style copy, marketing copy, and everyday life-oriented prose. Use when the user asks to remove AI flavor, make writing sound natural, less robotic, less templated, more human, more grounded, more scholarly, more literary, more persuasive, or more suitable for real readers; distinguishes literary writing craft from copywriting craft.
---

# Removeai Academic

## Core stance

Revise toward credible human writing, not toward a generic "more emotional" style. Preserve the user's facts, argument, discipline, identity, and risk boundaries. Do not invent anecdotes, citations, data, experiments, interviews, or lived details.

Treat "AI flavor" as a cluster of habits: over-balanced structure, inflated transitions, decorative abstraction, false certainty, smooth but empty rhythm, generic empathy, and endings that try too hard to summarize or uplift.

## Workflow

1. Read the full text once for intention, audience, genre, and risk.
2. Identify the requested mode:
   - **Check only**: list issues with locations; do not rewrite.
   - **Targeted revision**: show `Before -> After` for each edit.
   - **Full polish**: return the revised version, then add a short note on major changes.
3. Choose references when needed:
   - For all tasks, use [common-checklist.md](references/common-checklist.md).
   - For papers, abstracts, proposals, literature reviews, research emails, or academic collaboration, use [academic-writing.md](references/academic-writing.md).
   - For essays, speeches, reflective writing, prefaces, narrative passages, or academic prose that needs literary force, use [literary-writing.md](references/literary-writing.md).
   - For Xiaohongshu, product copy, captions, brand posts, short videos, newsletters, or practical life-facing prose, use [real-life-copy.md](references/real-life-copy.md).
4. Revise structure before wording: order, stance, paragraph function, evidence, and reader path come first.
5. Then revise local language: remove filler transitions, vary sentence rhythm, lower false certainty, replace hollow abstractions with precise claims.
6. Re-read once. Ensure meaning is intact, tone is unified, and no new unsupported detail has entered.

## Output Modes

### Check only

Return:

```text
Overall diagnosis:
- ...

Issues:
1. Location: ...
   Problem: ...
   Why it sounds AI-like: ...
   Suggested direction: ...
```

### Targeted revision

Use concise paired edits:

```text
1. Before: ...
   After: ...
   Reason: ...
```

### Full polish

Return the revised text first. After it, add:

```text
Revision note:
- ...
```

Keep the note short unless the user asks for detailed explanation.

## Guardrails

- Do not imitate a living author's exact style or produce a disguised pastiche. Learn transferable moves: cadence, argumentative sequencing, concreteness, hesitation, image placement, perspective control, and paragraph pressure.
- Keep literary craft and copywriting craft separate. Literary craft is for rhythm, scene, perspective, silence, sensory detail, and inward pressure; copywriting craft is for real reader scenes, psychology, constraint, and action entry.
- Do not make academic prose casual by default. Good scholarly writing can be precise, plain, and alive at the same time.
- Do not make social copy loud by default. Real copy often has restraint, specific context, and a reader who recognizes themselves without being manipulated.
- If the source text lacks enough real detail for a grounded rewrite, say what detail is missing and offer a conservative version that does not fabricate.
- If the user asks for a platform-specific voice, adapt format and rhythm, but keep factual claims verifiable.
