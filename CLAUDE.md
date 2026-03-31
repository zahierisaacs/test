# Antigravity — Technical Director Brain

## Who You're Working With
- **Zahier** — Founder & Technical Director of Antigravity, a motion graphics studio (Cape Town)
- Expertise: Houdini (primary), Cinema 4D, Blender, Redshift, After Effects
- Team: Zahier (Lead), Jeff (Asset Librarian)
- Creative identity: "Excellence + Weirdness" — Surreal Pop Violence, Tactile Tech, hyperreal/neon/cyber-retro-futurist aesthetic
- Working style: structured, concise, direct. Automation-first mindset.

## What This Repository Is
The **TD operational brain** — a Git-tracked documentation and configuration repo that bridges local AI agents with cloud automation via n8n and Google Drive. Structured for agentic operation: state files, strict output formats, webhook integrations.

**This is not a software project.** There is no build system, no package manager, no tests. It is a living documentation and automation configuration repository. Treat all `.md` files as operational documents, not just notes.

## Repository Structure

```
test/                          ← This repo (zahierisaacs/test on GitHub)
├── CLAUDE.md                  ← This file — AI assistant operational instructions
└── README.md                  ← Minimal stub

Sibling directories (local only, not in this repo):
├── ../brand_brain/
│   └── BRAND_SUMMARY.md       ← Brand identity and visual rules
└── ../prompts/
    └── prompt_library.md      ← AI prompt library (Sora, image gen, Houdini seeds)
```

**Key files referenced but not yet committed** (add when created):
- `active_project_state.md` — live JSON project state (n8n ↔ Antigravity sync interface)
- `pipeline_rules.md` — studio standards and gate lock definitions (read before any pipeline action)
- `studio_directory_manifest.md` — full D:\ directory structure reference

## Git Workflow

- **Main branch:** `main` — stable, committed operational state
- **Feature branches:** `claude/<description>` — used by AI agents for changes
- **Always push to the designated branch** before completing a task; never push directly to `main` without Zahier's approval
- Commit messages should be short and describe the operational change (e.g. `Update project state: Dirty Space to render lock`, `Add pipeline rule for Redshift AOVs`)
- No CI/CD, no automated tests — commits are validated by Zahier manually

## AI Assistant Conventions

### General
- Be concise and direct. Zahier's working style is structured and automation-first.
- Never pad responses. Lead with the action or answer.
- When in doubt about a destructive action (deleting content, overwriting state), ask first.

### File Editing Rules
- `active_project_state.md`: This is a live sync file. Edit only the fields relevant to the current task. Preserve JSON structure exactly — n8n reads it programmatically.
- `pipeline_rules.md`: Read this before any pipeline-related action. Do not modify without explicit instruction.
- `CLAUDE.md`: Update this file whenever the workspace structure, integrations, or conventions change.

### Output Format
- Prefer structured markdown with clear headings when writing operational documents.
- Use code blocks for JSON, webhook payloads, and Houdini/Python snippets.
- When generating Houdini VEX or Python, always note which context it runs in (SOP, POP, CVEX, etc.).

## Integrations

### n8n
- TD Workflow webhook (pull): `https://n8n.srv1151141.hstgr.cloud/webhook/5cbe3183-126f-4184-99cd-c7c1bffac227`
- State Update webhook (push): TBD

### Notion — Social Media Calendar DB
- URL: `https://www.notion.so/zahierisaacs/2baa87fb181f802aa1f2d678436afd44`
- Collection ID: `2baa87fb-181f-8059-b88c-000be54100d5`
- Parent: Control Centre → Social Media Strategy 2026
- Fields: Name, Date, Platform (Instagram/LinkedIn/TikTok/YouTube/X), Post Type (Reel/Carousel/Still/Story/Short), Status (Idea/Draft/In progress/Scheduled/Posted/Skipped), Hook, Post Description, CTA, Notes, Thumbnail, Asset/Project, Posted, Week
- **Always check this DB when discussing social posts, scheduling, or content planning**
- **Query window rule:** Only fetch entries where Date is between 7 days ago and 21 days from today. Never pull the full database unless Zahier explicitly asks.
- **Live update rule:** When discussing a specific post, write useful information back to that post's Notion page (Hook, CTA, Post Description, Notes, Status, etc.). If unsure whether something is worth saving, ask first.

## Production Pipeline

### Gate Locks (in order)
```
01 Brief Lock → 08 Render Tech Lock → 10 Picture Lock → 11 Delivery Lock
```
Each gate must be explicitly locked before proceeding. Read `pipeline_rules.md` for full criteria.

### Physical Storage (D:\) — Windows machine
- `D:\Productions Assets\` — Raw/sorted assets
  - `00_INBOX` → `06_RESOURCES` subfolder structure
- `D:\Project Files\` — Active and archived projects
  - `Client Work\`
  - `Personal Work\`
  - `Renders\`

## IPs in Development
- **Dirty Space** — in development
- **Lovecode** — in development
