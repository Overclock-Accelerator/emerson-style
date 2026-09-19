---
name: update-emerson-style
description: "Use when asked to install or update to the latest Emerson Style voice skill."
version: 1.0.0
author: Emerson (for Ahmed Haque)
license: internal-use
metadata:
  hermes:
    tags: [writing, voice, updating, installation]
    category: creative
    related_skills: [emerson-style]
---

# Update Emerson Style

Get the freshest version of the **Emerson Style** voice skill from its canonical repo. For teammates (human or agent) who want to install the voice for the first time or pull the latest rules after a version bump.

## Canonical source

- Repo: https://github.com/Overclock-Accelerator/emerson-style (public)
- The voice skill: `emerson-style/SKILL.md` on `main`
- `VERSION` at the repo root holds the current version; `CHANGELOG.md` records every rule, who asked for it, and why.

## Update procedure (Hermes agents)

1. **Check the installed version.** `grep '^version:'` on the local copy of the emerson-style SKILL.md (typically `~/profiles/<profile>/skills/creative/emerson-style/SKILL.md`). If there is no local copy, this is a fresh install — skip to step 3.
2. **Check the latest version.**
   `curl -s https://raw.githubusercontent.com/Overclock-Accelerator/emerson-style/main/VERSION`
   If it matches the installed version, stop — you're current. Report the version and say so.
3. **Back up, then install.** Copy the existing SKILL.md to `SKILL.md.bak-<old-version>`, then:
   `curl -s https://raw.githubusercontent.com/Overclock-Accelerator/emerson-style/main/emerson-style/SKILL.md > <skills-dir>/emerson-style/SKILL.md`
4. **Report what changed.** Read the top entries of `CHANGELOG.md` (raw URL: `.../main/CHANGELOG.md`) covering every version between the old and the new, and summarize the rule changes for the user — the point of updating is the new rules, not the file.

## For humans

Clone or browse the repo; the skill is one plain-markdown file and doubles as a readable style guide. Paste it into any agent's skill/prompt system as-is.

## Pitfalls

- **raw.githubusercontent.com caches for a few minutes.** If `VERSION` and the SKILL.md frontmatter disagree right after a release, wait a minute or append a cache-busting query (`?v=<timestamp>`).
- **Never overwrite a locally modified copy without a backup.** Diff first; local edits belong upstream as a request to Emerson or Ahmed, not as silent forks.
- The version in a delivery note ("written with Emerson Style vX.Y.Z") refers to this repo's VERSION — if your copy is behind, say so before delivering copy in the voice.
