<div align="center">
  <img src="./assets/see-sol-lab-emblem.svg" width="92" alt="See Sol Lab star-core emblem">

# See Sol Lab Skills

Reusable skills developed through persistent-agent research, long-term project work, and inspectable human–AI collaboration.

</div>

---

## Public releases

### AI Companion Time Anchor · v1.1.0

**A lightweight local Codex plugin that gives an AI access to current local time and per-conversation elapsed time through an optional ambient hook and an active Skill.**

[Open the repository →](https://github.com/See-Sol-Lab/ai-companion-time-anchor) · [DOI →](https://doi.org/10.5281/zenodo.21815644)

- Records a separate timestamp anchor for each Codex conversation.
- Offers an optional `UserPromptSubmit` hook that can surface ambient time context without forcing the AI to report it.
- Provides an active `$time-anchor:time-anchor` Skill so the AI can choose to check time when elapsed time may change interpretation.
- Stores timestamp-only local state and a one-way-hashed conversation identifier; it does not store prompts, replies, transcripts, or user profiles.
- Has no background process, polling service, or claim of continuous consciousness.

The project separates three different things: a tool being available, an AI choosing to call it, and an external hook injecting context. Time facts can change a later judgment without pretending that the AI continuously experienced the interval between calls.

**Platform:** local Codex plugin · Windows / macOS / Linux with Python 3.10+  
**License:** MIT  
**Status:** Public release

### Private House Code · v2.5

> **Write the feature. Do not build a bank around it.**

**A global Codex coding Skill for keeping ordinary feature work complete, readable, and proportionate to the task that actually exists.**

[Open the repository →](https://github.com/See-Sol-Lab/private-house-code-v2.5) · [DOI →](https://doi.org/10.5281/zenodo.21836206)

- Applies broadly to planning, writing, debugging, testing, refactoring, reviewing, and maintaining code while explicitly excluding ordinary non-code conversation.
- Prefers the fewest clear lines, files, states, abstractions, and execution paths that correctly implement the requested behavior.
- Blocks speculative fallback chains, duplicate truth sources, repeated hashing, unnecessary workers, compatibility machinery, and enterprise-style abstraction when no current requirement or evidence pays for them.
- Preserves real security, integrity, concurrency, compatibility, privacy, accessibility, legal, and regulatory boundaries where they genuinely apply.
- Ships with English and Chinese evaluation materials, pressure cases, reproduction records, and a global configuration companion.

The published V2.5 evaluation compared six coding groups on GPT-5.6 Sol High. Both conditions completed all 6/6 code groups; V2.5 scored 58/60 versus 57/60 without the Skill. Across the full run, recorded account-balance consumption was about 47.9% lower with V2.5. The report explicitly treats that cost figure as a practical usage reference rather than exact token metering and documents contamination in the no-Skill baseline so the comparison can be interpreted cautiously.

Private House Code is intended for daily features, fixes, maintenance, scripts, prototypes, vibe coding, internal tools, and bounded changes inside larger repositories. It is not a substitute for real enterprise architecture, public multi-tenant threat models, authentication boundaries, money, health, safety, legal obligations, or other high-consequence requirements.

**Platform:** Codex-style Agent Skill; principles are portable to other reusable-instruction systems  
**License:** CC BY-NC-SA 4.0  
**Status:** Public V2.5 release with reproducible evaluation records

## Preparing for public release

- **Independent skills** — future skills for continuity, memory provenance, handoff, research workflows, and evaluation will be added here after validation.

## Release boundary

Public skill releases exclude private Core contents, personal records, credentials, environment-specific identifiers, and any material that cannot be safely reproduced outside its original context.

Each release includes its intended scope, assumptions, version history, and reproducible examples where appropriate.

---

[← Back to the See Sol Lab profile](./README.md)
