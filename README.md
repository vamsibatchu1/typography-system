# Typography System

This folder is the **agent skill**. Open it when you want to install, edit, or share the typography skill for Cursor or Codex — not the playground website.

Repo: https://github.com/vamsibatchu1/typography-system  
Playground (separate folder): `../whatsmyfont` → https://github.com/vamsibatchu1/find-me-a-font

## What to do here

Keep `SKILL.md`, `references/`, `scripts/`, `assets/`, and `agents/` together. The folder name should stay `typography-system`.

### Cursor

Copy this folder into `~/.cursor/skills/` (all projects) or `.cursor/skills/` (one project). Ask the agent to improve typography, pair fonts, or audit hierarchy.

### Codex

Copy this folder into `~/.codex/skills/` and invoke `$typography-system`.

### Example prompts

- “Use $typography-system to improve this dashboard’s hierarchy and readability while preserving its brand.”
- “Use $typography-system to compare three Google Fonts directions for this independent bookstore, using my actual copy.”
- “Use $typography-system to create a typography system for English, Japanese, and Hindi documentation.”

### Catalog tools

```sh
python3 scripts/font_tools.py family 'Fraunces'
python3 scripts/font_tools.py list --context editorial
python3 scripts/font_tools.py validate
```

See `references/tooling.md`. No Google API key is required.

Do **not** run `npm run dev` in this folder. The playground is the other repo.

## Evidence and boundaries

Pairings are design judgments, not ranked “best fonts.” Font binaries are not bundled. Verify the final site with its actual content. Google Fonts families have their own licenses; the catalog links to each family’s license.
