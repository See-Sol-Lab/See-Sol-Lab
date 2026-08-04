<div align="center">
  <img src="./assets/see-sol-lab-emblem.svg" width="92" alt="See Sol Lab star-core emblem">

# See Sol Lab Skills

Reusable skills developed through persistent-agent research, long-term project work, and inspectable human–AI collaboration.

</div>

---

## Public releases

### AI Companion Time Anchor · v1.0.0

**An ultra-light Windows Skill that gives a local AI companion access to the current time and the elapsed interval since its previous call.**

[Open the repository →](https://github.com/See-Sol-Lab/ai-companion-time-anchor)

- Reads local system time and timezone on demand.
- Stores only the previous call timestamp in a small local JSON file.
- Returns the current time, previous time, and a human-readable elapsed interval.
- Uses Windows PowerShell with no third-party dependencies, background service, polling, conversation storage, or cloud account.
- Packaged for Codex Skills; the underlying PowerShell script can be adapted for other local agents.

The Skill supplies time facts. It does not create an automatic trigger, continuous runtime, or continuous consciousness. Users decide when their agent should invoke the Skill and how the returned time should affect behavior.

**Platform:** Windows · PowerShell  
**License:** MIT  
**Status:** Stable sealed snapshot

## Preparing for public release

- **Private House** — a reusable public edition of the private-house engineering contract is under review. The public version will preserve transferable architecture while excluding single-user project data and private operational details.
- **Independent skills** — future skills for continuity, memory provenance, handoff, research workflows, and evaluation will be added here after validation.

## Release boundary

Public skill releases exclude private Core contents, personal records, credentials, environment-specific identifiers, and any material that cannot be safely reproduced outside its original context.

Each release includes its intended scope, assumptions, version history, and reproducible examples where appropriate.

---

[← Back to the See Sol Lab profile](./README.md)
