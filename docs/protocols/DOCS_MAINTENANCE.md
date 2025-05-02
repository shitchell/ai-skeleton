# DOCS_MAINTENANCE.md

## 📘 Purpose
This file describes how documentation is maintained, pruned, and migrated across the lifecycle of development.

---

## 🧽 Pruning Guidelines
- Use the tag `<!-- prune-needed -->` in any file where outdated, redundant, or resolved information exists
- AI assistants are encouraged to emit pruning tags when they:
  - Repeat information already documented
  - Change direction mid-design
  - Migrate content into a more canonical location

---

## 🪵 Prune Triggers
- After each feature completion → run through [CYCLE_END_OF_FEATURE.md](./CYCLE_END_OF_FEATURE.md)
- After a full build passes → prune stale notes, diagrams, exploratory logs
- Before starting a new major feature or rewrite

---

## 📚 What Goes Where
- **PROJECT_SPECS.md** → long-term identity and intent
- **DEVELOPMENT_LOG.md** → chronological scratchpad of session plans and outputs
- **SCRATCH.md** → temporary holding area for miscellaneous items that need later attention
- **LESSONS_LEARNED.md** → postmortems and generalized takeaways
- **DESIGN_DECISIONS.md** → architecture commitments and rationale
- **IMPLEMENTATION_PLAN.md** → evolving plan for what's coming next

---

## 🗃 Archive Strategy
Move stale or unused materials to a folder like `docs/archived/` to avoid loss while improving active context clarity.

- Log the archival under `DEVELOPMENT_LOG.md`
- Ensure the reasons for archival are documented under `LESSONS_LEARNED.md` and `DESIGN_DECISIONS.md`

---

## 🔄 Navigation
- Return to [CYCLE_DEVELOPMENT_PROCESS.md](./CYCLE_DEVELOPMENT_PROCESS.md)


> 🔍 Check for gaps or rot in your dependency map using [MAP.md](../project/blueprint/MAP.md) and run [COHERENCE_CHECK.md](./COHERENCE_CHECK.md) for structural clarity.
