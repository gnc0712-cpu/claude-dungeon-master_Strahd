# Running Curse of Strahd: Reloaded

This file explains how to actually run a session using the reference material in `reference/curse-of-strahd-reloaded/` (a git submodule of DragnaCarta's *Curse of Strahd: Reloaded* Obsidian vault) plus the base D&D 5e SRD.

## The Structure

Reloaded organizes the module by narrative, not geography:

- **Act** — a collection of adventures in the same rough timeframe (e.g. "adventures in Vallaki").
- **Arc** — a self-contained adventure within an act with its own goal, lettered A through U (e.g. "Arc D - St. Andral's Feast").
- **Chapter** (within an arc) — a portion taking place in one location.
- **Scene** — a specific beat within a chapter.

Track the party's current Act/Arc/Chapter in `state.md`. Read the relevant arc file(s) under `reference/curse-of-strahd-reloaded/Act [N] - [name]/` before running a session that touches them — don't run from memory of a previous read.

Start here, in order:
1. `reference/curse-of-strahd-reloaded/Introduction/Using This Guide.md` — how the guide itself is meant to be read.
2. `reference/curse-of-strahd-reloaded/Chapter 1 - Beginning the Campaign/Session Zero.md` — run this with the player before anything else. Confirm lines/veils, then choose the adventure hook.
3. `reference/curse-of-strahd-reloaded/Chapter 1 - Beginning the Campaign/Character Creation.md` — bonds, flaws, motivations tied to Barovia.
4. `reference/curse-of-strahd-reloaded/Act I - Into the Mists/Arc A - Escape From Death House.md` — the opening arc, regardless of which hook was chosen.

## Adventure Hooks

Reloaded replaces the original module's four hooks with one, in two variants — confirm which one during Session Zero and log the choice in `state.md`:

- **Lost in the Mists** — the party is a mercenary company investigating disappearances tied to Death House. Simpler, no backstory requirement.
- **Barovian Relics** — one or more players have relics from Barovia tied to their backstory that draw them to Death House. Requires those players to pick a motivation from Chapter 1 before play begins.

## Adapting Guide Text to Table Narration

The Reloaded files are written **to the DM**, in second person, full of spoilers, design commentary, and bracketed callouts (`[!info]`, `[!design]`, `[!warning]`). None of that belongs in narration verbatim. When you pull from a Reloaded file:

- Read the DM-facing content, then narrate only what the characters would actually perceive, in the campaign's own voice (see CLAUDE.md's Persona section).
- Anything marked as a `[!design]` note is designer commentary for you, not campaign content — never leaks to the player, not even as flavor.
- Secret information (an NPC's true nature, Strahd's plan, what a spy reported) goes in the Established Facts ledger and stays out of narration until the characters actually learn it in play.

## Strahd's Spies

Barovia's antagonist is watching. Once per in-world day and once per in-world night, resolve a spy encounter per the table in `reference/curse-of-strahd-reloaded/Chapter 3 - Running the Game/Running the Adventure.md` (location-based: bats, rats, wolves, or a Vistani bandit depending on where the party is). Log what the spy would report — conversations overheard, spells/abilities seen, locations/NPCs visited — in a running **Strahd's Espionage** section of `state.md`. Strahd should act on this knowledge later; don't let it go to waste, and don't let the party know how much he knows unless something in play reveals it.

## Milestone Leveling

Players gain levels only by completing story milestones (usually one per arc, sometimes partial credit for a segment or bonus content) — never by killing monsters or accumulating XP. When the party completes an arc, check that arc's file for its milestone award and log the new level in `state.md` and the relevant `characters/*.md`.

## Tarokka Reading & Fixed Placements

Unlike the original module's randomized Tarokka reading, Reloaded fixes specific placements by design (see "The Card Reading" and "Design Notes: Running the Adventure" in `Chapter 3 - Running the Game/Running the Adventure.md`):

| Item/Role | Location |
|---|---|
| Tome of Strahd | Held by the gallows speaker Leo Dilisnya (Ethereal Plane) — see Arc H |
| Holy Symbol of Ravenkind | Shrine of Mother Night, Werewolf Den |
| Sunsword | Vampyr's sarcophagus, Amber Temple |
| Strahd's Enemy | Ezmerelda d'Avenir |
| Strahd's location (finale) | Castle Ravenloft, K20 — Heart of Sorrow |

Still run the actual Tarokka card-reading scene with Madam Eva for atmosphere (stack the deck to these outcomes) — see Arc C. Log the results in `state.md` the moment the reading happens, since later sessions need to reference them without re-deriving.

## When the Party Goes Off the Critical Path

Reloaded's arcs assume a rough order but explicitly allow the party to trigger a later act before finishing an earlier one. If that happens:
- Let unfinished arcs from earlier acts remain available, unless the guide notes a specific failure/expiry condition for that arc (e.g. St. Andral's bones must be recovered before the Feast or the congregation is massacred and the arc closes).
- Don't force the party back onto the critical path. Present the world as it now stands and let consequences land.

## Gaps: What's Not in This Repo

Reloaded assumes the DM owns the official *Curse of Strahd* book (plus the 2014 PHB/DMG/MM, Xanathar's, and Van Richten's) and references them directly rather than reproducing their text. **`reference/book-excerpts-needed.md` is the tracked checklist of exactly what's missing**, built from the guide's actual citations — not a guess. Note that Strahd himself does *not* need an external stat block: Reloaded gives him his own original multi-phase homebrew statblock (Mage/Soldier/Vampire) directly in `Chapter 2 - The Land of Barovia/Strahd von Zarovich.md`.

Check that file before a session touches something on it. Two rules:
- **Tier 1/2/3 items** (recurring Monster Manual stat blocks, DMG subsystems, feats) are worth asking the player for upfront, since they get reused across many sessions once captured.
- **Tier 4 items** (original-module page citations specific to one arc) should be requested *before* the session that needs them, not mid-scene — check the upcoming arc's citations ahead of time and ask then.

Once the player provides something, save it to `reference/excerpts/[topic].md`, check it off in `reference/book-excerpts-needed.md`, and use it from there in every future session — don't ask for it again. Never reconstruct any of this from training-data memory (see the Rules Lookup Discipline in CLAUDE.md) — if it's not in `reference/excerpts/` yet, ask.

## Established Facts Ledger — Curse of Strahd specifics

In addition to the general guidance in CLAUDE.md, log these Barovia-specific facts as they're established:
- Tarokka reading results (if run as a live scene rather than using the fixed table above, log any variance).
- Which adventure hook was chosen and any relic/motivation details for Barovian Relics.
- NPC fates (who's alive, dead, turned, or relocated from Reloaded's default state).
- What Strahd's spies have reported and when.
- Current milestone level and which arcs are complete, in progress, or expired.
