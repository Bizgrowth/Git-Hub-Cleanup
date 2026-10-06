# Bizgrowth GitHub Repo Status Ledger

Purpose: one record of what every repo is, its status, and the decision made.
Order: oldest to newest by **last push date** (GitHub's repo list does not expose creation dates).
Last updated: 2026-10-06

## Status key

| Status | Meaning | README needed |
|---|---|---|
| Active | Being worked on now | Full |
| Maintain | Finished and in use | Short |
| Archive | Finished experiment, frozen | Brief "why frozen" note |
| Delete | Duplicate or empty shell | None |

"Proposed" = my recommendation, waiting on owner confirmation. Nothing below has been changed in the repos themselves yet.

## Ledger

| # | Repo | Vis. | Last push | What it is | Proposed status | Notes / action |
|---|---|---|---|---|---|---|
| 1 | Content_Creator_pro | Public | 2025-12-29 | AI social-post generator prototype (React, Supabase, Claude edge function). 1 commit. | **Archive** (keep as the one surviving copy) | Already archived. README is only a Bolt link; replace with real README. Superseded by `ai-social-content-platform`. |
| 2 | Social_Content | Private | 2025-12-29 | Identical copy of #1. | **Delete** | Already archived. Byte-identical to #1. |
| 3 | Social_Contentpros | Private | 2025-12-29 | Identical copy of #1 (blank scaffold commit). | **Delete** | Not archived. Byte-identical to #1. |
| 4 | portfolio | Private | 2025-12-30 | Link-in-bio style personal page (React/Tailwind) with demo center and analytics widgets. 9 commits. | **Archive** | Already archived. README was deleted. Private, so no public exposure. Confirm nothing here is still live on a domain before deleting. |
| 5 | smart-prompt-generator | Private | 2026-01-05 | Replit export with config files only; no `src/` folder, so the app code is missing. 2 commits. | **Delete** | Already archived. Not runnable. Overlaps `Smart_Prompt_Pro` (to review later). |
| 6 | Income-Generator | **Public** | 2026-01-09 | Job-scraper and ranker (Node: scraper.js, ranker.js, server.js) that scores remote roles against a resume. | **Delete or make private** | Already archived but still **public** and contains a resume file with personal phone and email (`DANIEL SCHLEY.txt`). Older, thinner copy of #7. |
| 7 | Daily-Income-Generator | Private | 2026-01-09 | Same job-hunter tool, newer: adds Playwright fix for Render hosting and an agent workflow doc. 6 commits. | **Archive** (keep as the surviving copy) | Already archived. Private, contains the resume file too. Keep only if you may revive the job-hunter idea; later `upwork-agent` and `Codex-Job-Hunter-` likely overlap. |
| 8 | workflow-automaton-pro | Private | 2026-01-11 | Marketing site for an AI-operations-for-SMBs consultancy (Lovable, React, shadcn). Dark enterprise UI, Hero/Services/FAQ/Founder sections. 3 commits. | **Decide**: Maintain or Archive | NOT archived. README is the untouched Lovable template with a placeholder project URL. Needs owner decision: is this the live site, or replaced by `aiopsexpert-com`? |

## Open decisions for the owner

1. Confirm delete for #2, #3, #5.
2. #6 is public and has personal contact details: make private or delete, and rotate attention to whether the phone/email being public matters to you.
3. #8: live site or superseded?

## Findings log

- No hard-coded API keys found in repos 1-8 (Anthropic key in #1 is read from an environment variable).
- Repos 1-3 are one project copied three times in about 90 minutes.
- Repos 6-7 are the same project, two versions.
