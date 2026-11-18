# Elena agent — a personal model that learns a person (working name)
Started 2026-11-12. Owner: Elena Chrysaki. Status: concept + daily research.

## The idea
An agent (later open source) that learns ONE person over time:
1. how they speak and mean things (per language: Greek vs English),
2. their design taste and where it comes from (environment, experiences),
3. their processes and decisions,
4. the mistakes made together, turned into rules.
It learns mostly from the gap between a person's first ask and their final decision, and it evolves with them:
taste levels up slowly; the model must weight recent confirmed signals, keep history, and never freeze the person.
Privacy: local-first, user-owned, private sandbox; minimal-token sync to any AI tool (Claude, Codex…) via plugin/MCP.

## Live prototype
`~/.claude/elena/` — README, design, about, voice, mistakes, changelog. Weekly consolidation task (Sundays).

## Research questions (daily task rotates through these)
1. Human thought & neurology: how memory, association, attention and decisions work; why people like what they like.
2. Language: how speaking differs between languages (Greek vs English), bilingual thinking, implicature — saying vs meaning.
3. Context, memory, experience: how they shape perception, taste and choices.
4. Design & environment: how surroundings, culture, era and media shape aesthetics and decisions.
5. AI memory: how agents store, retrieve, forget, consolidate; personal memory tools (Mem0/OpenMemory, Letta, Zep, memory-mcp…).
6. Tracking good decisions + evolving taste: preference drift, recency weighting, versioned profiles, confirmed vs inferred.
7. Out-of-the-box connections: hidden links between unrelated likes (e.g. "why number 2 and number 6?").

## Known landscape (2026-11-12)
- Generic user-owned memory exists (Mem0 OpenMemory MCP, memory-mcp, personal-memory-mcp). Facts, not taste/voice.
- Taste-from-feedback exists inside teams (LangChain Content Studio: fast feedback log + slow consolidation loop). No open, person-level product found.
- Gap = taste + voice + biography + mistakes-as-rules, learned from first-ask→final-decision diffs, portable and private.

## Files
- research/YYYY-MM-DD.md — one note per day (sources, findings, ideas for the agent, next questions).
- research/INDEX.md — one line per day.
- cases/ — real design decisions traced from first ask to final choice, with what the agent should learn (e.g. 2026-11-13-top-form-hero.md).

## Key insight (2026-11-12): how humans actually mean things
People connect ideas through hidden sensory stimuli, not just logic. Elena's examples:
- 2 and 6 are liked because they feel glossy, curved and fluid ("drawn in water, dripping like honey"), and because even numbers can be split many ways.
- "Lighter" = a feather: soft and fragile, no tension, effortless. Glass is hard and fragile, so it is the wrong metaphor.
The agent must (1) find the hidden link behind loosely connected sentences, (2) store metaphors as specs with what they ARE and are NOT, and (3) ask in sensory language ("what material does it feel like?").

## Design note (2026-11-12): privacy tiers
Profiles need tiers: shareable taste/voice vs a private wellbeing tier that is never synced, exported or loaded by default, only read when the person raises something personal. Store how to help, never event details.
