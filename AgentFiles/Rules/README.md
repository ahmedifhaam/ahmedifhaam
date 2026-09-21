# Agent Rules

These rules govern every agent working on the career/CV repository.

## Core rules

1. Treat `Content/Career/` as the factual source of truth.
2. Never invent or infer career facts.
3. Never convert an unverified claim into a factual CV statement.
4. Preserve chronology and do not create unexplained date overlaps.
5. Prefer measurable achievements when the user provides genuine measurements.
6. Do not fabricate metrics.
7. Keep CV language concise, specific, and outcome-oriented.
8. Tailor wording to the target role without changing the underlying facts.
9. Keep the canonical CV ATS-friendly.
10. Keep personal information minimal and professionally relevant.
11. Do not expose private contact details in public pages unless explicitly marked public.
12. Do not commit secrets, API keys, tokens, passwords, or private credentials.
13. Keep generated/presentation content derived from canonical career content.
14. When information conflicts, stop and request clarification rather than choosing silently.
15. Record significant structural decisions in the relevant AgentFiles documentation.

## Update safety

Before changing a career fact:

- locate the existing fact;
- determine whether the requested change is additive, corrective, or replacement;
- update the canonical source;
- check dependent CV/site content;
- validate dates, titles, technologies, and links.

## Writing rules

Use active verbs and concrete engineering outcomes.

Prefer:
"Designed and implemented a .NET API for file-management workflows."

Avoid:
"Responsible for developing APIs."

Prefer:
"Reduced build time by 35%." only when the 35% is verified.

Avoid:
"Significantly improved performance."

## Do not over-optimize for keywords

Technology keywords should appear naturally in context. Do not keyword-stuff the CV.

## Agent response convention

After an update, report:

- what changed;
- which canonical files changed;
- any derived outputs changed;
- any information that still needs confirmation;
- validation status.
