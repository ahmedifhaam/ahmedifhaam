# Ahmed Ifhaam — Career & CV

This repository is the single source of truth for maintaining Ahmed Ifhaam's professional CV/resume and its public presentation.

## Repository principles

- **AgentFiles/** contains the operating system for agents: skills, rules, standards, workflows, and templates.
- **Content/** contains career facts, experience, projects, education, skills, achievements, assets, and CV source content.
- **README.md** is the human/agent navigation guide.

The repository should remain structured, factual, maintainable, ATS-friendly, and suitable for publishing as a static GitHub Pages site.

## Root structure

```
.
├── AgentFiles/
│   ├── Rules/
│   ├── Standards/
│   ├── Skills/
│   ├── Templates/
│   └── Workflows/
├── Content/
│   ├── Career/
│   ├── Assets/
│   ├── CV/
│   └── Resources/
└── README.md
```

## Source-of-truth model

Career facts belong in `Content/Career/`. Generated CVs, website pages, PDFs, and other presentation outputs must be derived from that content rather than becoming independent sources of truth.

Agents must never invent employment dates, technologies, responsibilities, achievements, metrics, qualifications, or links. If information is missing, mark it as missing and ask for confirmation.

## Updating the CV from ChatGPT

The intended workflow is:

1. Tell ChatGPT what changed, for example: "I joined X as Senior Software Engineer" or "Add this project to my CV."
2. The career agent reads the relevant AgentFiles rules and the existing Content/Career data.
3. The agent updates the canonical career content.
4. The agent updates derived CV/site content when appropriate.
5. The agent validates consistency, dates, wording, links, and formatting.
6. The changes are committed to this repository.

ChatGPT is therefore an editing interface to this repository, while the repository remains the source of truth.

## Website

The public CV should be publishable through GitHub Pages. The site should provide:

- professional profile/summary
- experience
- selected projects
- skills
- education/certifications
- links
- a clear **Download CV** action
- a responsive mobile layout
- accessible semantic HTML
- ATS-friendly CV content

The existing `ahmedifhaam.github.io` repository is currently the public Pages repository. This repository can first act as the content/source repository; the public site can later be migrated here or generated from this repository.

## CV design direction

Use a modern software-engineering style:

- white/light neutral background
- black/dark charcoal text
- one restrained accent colour
- strong typography and spacing
- no skill bars or star ratings
- no unnecessary icons or decorative graphics
- no photo unless specifically required for a target market
- one-column ATS-safe CV as the canonical format
- two pages are acceptable when experience warrants it

## Agent entry point

Start with:

- `AgentFiles/Rules/README.md`
- `AgentFiles/Standards/CV_STANDARD.md`
- `AgentFiles/Workflows/UPDATE_CV.md`
- `AgentFiles/Templates/CV_TEMPLATE.md`
- `Content/Career/README.md`

## Change discipline

Every material career update should preserve a clear history through Git commits. Do not silently overwrite facts. Prefer small, focused changes.

