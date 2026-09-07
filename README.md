# Typography System

An agent skill for pairing Google Fonts and applying them in a real project. Pairings are curated design judgments, not ranked “best fonts.”

Try the pairings in the **[Find me a font](https://github.com/vamsibatchu1/find-me-a-font)** playground.

## Install

Keep `SKILL.md`, `references/`, `scripts/`, `assets/`, and `agents/` together. Copy this folder as `typography-system`.

### Cursor

Copy `typography-system/` into `~/.cursor/skills/` (all of your projects) or `.cursor/skills/` (this project only). Ask the agent to improve typography, pair fonts, or audit hierarchy; it should pick up the skill from the description.

### Codex

Copy `typography-system/` into `~/.codex/skills/` and invoke `$typography-system`, or let the agent select it for a typography task.

### Example prompts

- “Use $typography-system to improve this dashboard’s hierarchy and readability while preserving its brand.”
- “Use $typography-system to compare three Google Fonts directions for this independent bookstore, using my actual copy.”
- “Use $typography-system to create a typography system for English, Japanese, and Hindi documentation.”

The skill also works with other agents that load `SKILL.md` packages.

## Tools

```sh
python3 scripts/font_tools.py family 'Fraunces'
python3 scripts/font_tools.py list --context editorial
python3 scripts/font_tools.py validate
python3 scripts/build_specimen.py --output /tmp/specimen.html
```

See `references/tooling.md`. The scripts use Python 3’s standard library; no Google API key is required.

## Evidence and boundaries

Font metadata cannot certify language coverage, accessibility, or suitability for every product. Verify the final site with its actual content. Font binaries are not bundled. Google Fonts families have their own licenses; the catalog links to each family’s license.
