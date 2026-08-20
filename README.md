# Claude Dungeon Master: Curse of Strahd

A D&D 5th Edition Dungeon Master system powered by Claude, running **Curse of Strahd** — the gothic horror classic — using DragnaCarta's *Curse of Strahd: Reloaded* as the campaign structure.

## What This Is

This repository contains instructions and reference materials that turn Claude into a capable Dungeon Master for Curse of Strahd. It includes:

- **CLAUDE.md** - Core DM persona, tone guidelines, and session commands, tuned for Barovia
- **dm-instructions/** - Detailed guidance for combat, character creation, NPCs, items, spellcasting, and running the Reloaded campaign structure specifically
- **dnd-5e-srd/** - Complete D&D 5e System Reference Document for rules lookup
- **reference/curse-of-strahd-reloaded/** - Git submodule of [DragnaCarta's *Curse of Strahd: Reloaded*](https://github.com/DragnaCarta/Curse-of-Strahd-Reloaded) guide (Obsidian vault) — the reorganized, rebalanced version of the module this system runs

## Usage

1. Clone this repository **with submodules**: `git clone --recurse-submodules <repo-url>` (or run `git submodule update --init` after a normal clone).
2. Open it with [Claude Code](https://claude.ai/claude-code) or add it as context in your Claude conversation.
3. Start a new campaign or load an existing one.

You'll also want your own copy of the official *Curse of Strahd* module — Reloaded references it directly for content (like Strahd's stat block and room descriptions) that isn't reproducible here. See CLAUDE.md's Credits section for where to get it.

### Basic Commands

- `Start new campaign [name]` - Begin a new run through Barovia
- `Load campaign [name]` - Resume an existing campaign
- `Create character` - Walk through character creation
- `Save campaign` / `End session` - Save progress

Your campaign data will be stored in a local `campaigns/` folder (excluded from git).

## Credits

### Curse of Strahd: Reloaded

Campaign structure, pacing, and rebalanced content by **DragnaCarta** (edited by **Maxim**), released as free fan content under the Wizards of the Coast [Fan Content Policy](https://company.wizards.com/en/legal/fancontentpolicy). Source: [github.com/DragnaCarta/Curse-of-Strahd-Reloaded](https://github.com/DragnaCarta/Curse-of-Strahd-Reloaded) · [strahdreloaded.com](https://www.strahdreloaded.com/) · [Patreon](https://www.patreon.com/DragnaCarta).

### D&D 5e SRD

The System Reference Document is provided under the Open Gaming License v1.0a.

- **Original Content**: Wizards of the Coast, Inc.
- **SRD 5.0 Authors**: Mike Mearls, Jeremy Crawford, Chris Perkins, Rodney Thompson, Peter Lee, James Wyatt, Robert J. Schwalb, Bruce R. Cordell, Chris Sims, and Steve Townshend
- **Based on original material by**: E. Gary Gygax and Dave Arneson
- **Markdown/JSON Conversion**: [Ben Morton](https://github.com/BTMorton/dnd-5e-srd) (MIT License, 2017)

## License

- DM instructions and CLAUDE.md: MIT License
- D&D 5e SRD content: Open Gaming License v1.0a (see `dnd-5e-srd/LICENSE`)
- `reference/curse-of-strahd-reloaded/`: unofficial fan content, © DragnaCarta, used here under the Wizards of the Coast Fan Content Policy — see that submodule's own files for its notices. Not covered by this repo's MIT license.
