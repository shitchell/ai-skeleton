# DEVELOPMENT_PROCESS.md

## 🔁 Iteration Cycle
This is the core loop used during daily AI-assisted development. If you're beginning work, start here.

---

### 🧭 1. Initialize
- Review [PROJECT_SPECS.md](../project/identity/PROJECT_SPECS.md) to reground in purpose and constraints
- Review [DEVELOPMENT_LOG.md](../project/workspace/DEVELOPMENT_LOG.md) for last session's status
- Review open `TODO`s or unresolved questions
- Validate current position in the project map using [MAP.md](../project/blueprint/MAP.md)

---

### 🧠 2. Plan
- Choose up to 3 components or tasks to implement
- Prioritize based on dependency order and current focus
- Log your plan at the top of [DEVELOPMENT_LOG.md](../project/workspace/DEVELOPMENT_LOG.md)
- Review and update [MAP.md](../project/blueprint/MAP.md) to ensure your planned work connects to project goals

---

### 🔍 2b. Coherence Validation
- Run [COHERENCE_CHECK.md](./COHERENCE_CHECK.md) to validate that your plan connects to the project goals
- Ensure each planned task:
  - Serves a clear project goal
  - Connects to existing components via the dependency chain
  - Has clear acceptance criteria that can be traced back to requirements
- Resolve any gaps identified by adding to [FLEX_POINTS.md](../project/blueprint/FLEX_POINTS.md) if needed

---

### 🛠️ 3. Implement
- Write modular code with composability and testability in mind
- Add type hints, logging, and inline docs as needed
- Justify design deviations directly in [DEVELOPMENT_LOG.md](../project/workspace/DEVELOPMENT_LOG.md)
- For significant shifts in approach, re-confirm coherence against [MAP.md](../project/blueprint/MAP.md)

---

### 🧪 4. Test
- Write minimal viable unit/integration/UI tests
- Include clear test case names and expectations
- Ensure test cases align with requirements in [MAP.md](../project/blueprint/MAP.md)
- Record results in [DEVELOPMENT_LOG.md](../project/workspace/DEVELOPMENT_LOG.md)

---

### 🧹 5. Diagnose and Refine
- Identify and log error types
- Trace root causes, document insights in [DEVELOPMENT_LOG.md](../project/workspace/DEVELOPMENT_LOG.md)
- If insights are complete and ready for permanent documentation, add to [LESSONS_LEARNED.md](../project/workspace/LESSONS_LEARNED.md)
- If insights need further reflection or don't fit elsewhere, add to [SCRATCH.md](../project/workspace/SCRATCH.md) with appropriate references
- Refactor for clarity, simplicity, and resilience
- For significant changes, update [MAP.md](../project/blueprint/MAP.md) to reflect new understanding

---

### 🧽 6. Prune
- Tag any outdated, redundant, or unclear content with: `<!-- prune-needed -->`
- Add pruning notes to [DEVELOPMENT_LOG.md](../project/workspace/DEVELOPMENT_LOG.md)
- Schedule review of large/messy documents if needed in `TODO.md`
- Use [VALIDATION.md](../VALIDATION.md) for linting and formatting checks

---

### ✅ 7. Review and Decide
- Does the result match project values and spirit?
- Does this implementation introduce new constraints or flex points?
- Do any new undefined fracture points need to be logged?
- Run [COHERENCE_CHECK.md](./COHERENCE_CHECK.md) to verify the implementation maintains system coherence
- Consider running [SYSTEM_AUDIT.md](./SYSTEM_AUDIT.md) for system-wide integrity checks if broader changes were made

---

### 📘 8. Close the Loop
- Update progress at the bottom of [DEVELOPMENT_LOG.md](../project/workspace/DEVELOPMENT_LOG.md)
- Update [MAP.md](../project/blueprint/MAP.md) to reflect the final state of the implementation
- If feature work is incomplete, return to step 1
- If feature is complete, continue to [CYCLE_END_OF_FEATURE.md](./CYCLE_END_OF_FEATURE.md)

---

### 🔄 Navigation
- Return to [PROJECT_SPECS.md](../project/identity/PROJECT_SPECS.md)
- If feature is complete, go to [CYCLE_END_OF_FEATURE.md](./CYCLE_END_OF_FEATURE.md)