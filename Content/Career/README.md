# Career Content

This directory is the canonical career knowledge base.

## Structure

```
Career/
├── Profile/
├── Experience/
├── Projects/
├── Skills/
├── Education/
├── Certifications/
└── Achievements/
```

Each branch should contain focused Markdown/YAML/JSON files rather than one giant career document.

## Rules

- Facts only.
- One source of truth per fact.
- Keep dates explicit.
- Use ISO dates where machine processing benefits from them.
- Mark uncertain information as `NEEDS_CONFIRMATION`.
- Keep public/private contact data clearly separated.

## Branching model

The career tree is intentionally hierarchical:

```
Career
├── Profile
├── Experience
│   ├── Current
│   └── Previous
├── Projects
│   ├── Backend
│   ├── Frontend
│   ├── Mobile
│   ├── Infrastructure
│   └── AI
├── Skills
├── Education
└── Certifications
```

Agents should update the smallest relevant branch and avoid flattening the career into one large file.
