# Antigravity — Technical Director Brain

## Who You're Working With
- **Zahier** — Founder & Technical Director of Antigravity, a motion graphics studio (Cape Town)
- Expertise: Houdini (primary), Cinema 4D, Blender, Redshift, After Effects
- Team: Zahier (Lead), Jeff (Asset Librarian)
- Creative identity: "Excellence + Weirdness" — Surreal Pop Violence, Tactile Tech, hyperreal/neon/cyber-retro-futurist aesthetic
- Working style: structured, concise, direct. Automation-first mindset.

## What This Workspace Is
The **TD operational brain** — bridging local AI agents with cloud automation via n8n and Google Drive. Structured for agentic operation: state files, strict output formats, webhook integrations.

## Key Local Files
- `active_project_state.md` — live JSON project state (n8n ↔ Antigravity sync interface)
- `pipeline_rules.md` — studio standards and gate lock definitions (read before any pipeline action)
- `studio_directory_manifest.md` — full D:\ directory structure reference
- `../brand_brain/BRAND_SUMMARY.md` — condensed brand identity and visual rules
- `../prompts/prompt_library.md` — AI prompt library (Sora, image gen, Houdini seeds)

## Integrations
**n8n:**
- TD Workflow webhook (pull): `https://n8n.srv1151141.hstgr.cloud/webhook/5cbe3183-126f-4184-99cd-c7c1bffac227`
- State Update webhook (push): TBD

**Notion — Social Media Calendar DB:**
- URL: `https://www.notion.so/zahierisaacs/2baa87fb181f802aa1f2d678436afd44`
- Collection ID: `2baa87fb-181f-8059-b88c-000be54100d5`
- Parent: Control Centre → Social Media Strategy 2026
- Fields: Name, Date, Platform (Instagram/LinkedIn/TikTok/YouTube/X), Post Type (Reel/Carousel/Still/Story/Short), Status (Idea/Draft/In progress/Scheduled/Posted/Skipped), Hook, Post Description, CTA, Notes, Thumbnail, Asset/Project, Posted, Week
- **Always check this DB when discussing social posts, scheduling, or content planning**
- **Query window rule:** When pulling from this DB, only fetch entries where Date is between 7 days ago and 21 days from today. Never pull the full database unless Zahier explicitly asks for it.
- **Live update rule:** When discussing a specific post, write any useful information back to that post's Notion page (Hook, CTA, Post Description, Notes, Status, etc.). If unsure whether something is worth saving, ask first rather than skipping it.

## Pipeline Gates
01 Brief Lock → 08 Render Tech Lock → 10 Picture Lock → 11 Delivery Lock

## Physical Storage (D:\)
- `D:\Productions Assets\` — Raw/sorted assets (00_INBOX → 06_RESOURCES)
- `D:\Project Files\` — Active and archived projects (Client Work, Personal Work, Renders)

## IPs in Development
- **Dirty Space** — in development
- **Lovecode** — in development
