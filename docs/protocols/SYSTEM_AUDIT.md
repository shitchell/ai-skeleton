# SYSTEM_AUDIT.md

## 🧭 Purpose

This file defines the protocol for validating the *project system itself* — its processes, relationships, and documentation — to ensure that all parts are:

- Internally coherent
- Functionally complete
- Free of dead ends or contradictory logic

This is the **coherence check for the coherence system** — a periodic meta-audit that ensures long-term structural integrity.

---

## 🔄 When to Run System Audit

- Once at the end of setup
- Before each milestone
- After adding or modifying any process document
- After completing a feature that introduced process changes (see [CYCLE_END_OF_FEATURE.md](./CYCLE_END_OF_FEATURE.md))
- When experiencing friction or confusion with existing processes
- When integrating new tools or methodologies into the workflow
- Anytime something feels "uncertain" about the system itself

---

## 🧪 Audit Protocol

### 1. System Process Coherence Testing

This section focuses on the coherence of the process framework itself.

#### 1.1 Process Mapping Validation

Check that the [PROCESS_ARCHITECTURE.md](./PROCESS_ARCHITECTURE.md) document accurately represents:

- All existing protocols and their relationships
- Clear entry and exit points for each process
- Explicit triggers between interconnected processes

Test Questions:
- Can every process be traced on the process map?
- Are there any processes referenced that don't exist?
- Are there any processes that exist but aren't represented?

#### 1.2 Cross-Reference Integrity

Verify that cross-references between documents are bidirectional and consistent:

- If Document A references Document B, Document B should acknowledge this relationship
- The nature of relationships should be consistent across both documents

Test Questions:
- For each reference to another document, does that document acknowledge this connection?
- Are there conflicting descriptions of how documents relate to each other?

#### 1.3 Dependency Cycle Detection

Identify any circular dependencies between processes:

- Document A → Document B → Document C → Document A
- Unresolvable chicken-and-egg scenarios

Test Questions:
- Can you trace a path that returns to the starting document without resolution?
- Are there decision points that rely on future information?

#### 1.4 Protocol Completeness

Each protocol must have:
- A clearly defined purpose and trigger
- An entry and exit point
- Linked references to related docs (and the links must resolve)
- No overlap or contradiction with other protocols

---

### 2. System Coverage Validation

Ensure that all necessary workflow states have a defined process:

- Project initialization to completion
- Error and exception handling
- Documentation maintenance

Test Questions:
- Is there a clear process for every state in the project lifecycle?
- Are there any "what if" scenarios that don't have a defined process?
- Are there clear exit criteria for each process?

Verify every type of project event is covered by at least one protocol:
- Initial planning
- Daily dev loop
- Feature completion
- Project closure
- Unexpected learning or pivot

Reference [PROCESS_ARCHITECTURE.md](./PROCESS_ARCHITECTURE.md) to confirm complete process coverage.

---

### 3. Constraint Consistency

Verify that constraints and rules are consistent across the system:

- Documentation conventions
- Decision-making criteria
- Quality standards

Test Questions:
- Are there contradictory rules in different documents?
- Are constraints consistently applied throughout related processes?

---

### 4. Project Structure Integrity

#### 4.1 MAP.md Validation

- All documents referenced by the map must exist
- Each node in [MAP.md](../project/blueprint/MAP.md) must be traceable to:
  - A goal ([PROJECT_SPECS.md](../project/identity/PROJECT_SPECS.md))
  - A blueprint ([COMPONENT_ARCHITECTURE.md](../project/blueprint/COMPONENT_ARCHITECTURE.md))
  - A downstream output ([DEVELOPMENT_LOG.md](../project/workspace/DEVELOPMENT_LOG.md), code, etc)

#### 4.2 Flex Point Lifecycle

- Every unresolved node must be:
  - Documented in [FLEX_POINTS.md](../project/blueprint/FLEX_POINTS.md)
  - Traced from a known file (not an orphaned thought)
  - Assigned a risk level + resolution timeline

#### 4.3 Implementation Traceability

Verify that all recommended practices are traceable to concrete implementation:

- Tools cited should have corresponding usage guidelines
- Processes should have specific entry points in codebases or documentation

Test Questions:
- Are tools and methods referenced with specific implementation details?
- Are abstract concepts connected to concrete artifacts?

---

### 5. Documentation Technical Validation

- Run:
  - `lychee docs/` for dead links
  - `markdownlint` for formatting
  - `vale` (if configured) for writing clarity
- Ensure all Markdown references are actual `[links](...)`, not inline filenames
- See [VALIDATION.md](../VALIDATION.md) for complete validation tools and procedures

---

## 📊 Audit Results Format

System audit results should be documented using this comprehensive format:

```markdown
## System Audit Results: YYYY-MM-DD

### Process Coherence
- [✅|⚠️|❌] Process mapping completeness
- [✅|⚠️|❌] Cross-reference integrity 
- [✅|⚠️|❌] Dependency cycles
- [✅|⚠️|❌] Protocol completeness

### System Coverage
- [✅|⚠️|❌] Workflow state coverage
- [✅|⚠️|❌] Event type coverage
- [✅|⚠️|❌] Constraint consistency

### Documentation Integrity
- [✅|⚠️|❌] MAP.md traceability
- [✅|⚠️|❌] Flex point documentation
- [✅|⚠️|❌] Implementation traceability
- [✅|⚠️|❌] Technical validation

### Issues Requiring Resolution:
1. [Issue description and location]
2. [Issue description and location]

### Improvement Opportunities:
1. [Opportunity description]
2. [Opportunity description]
```

For specific coherence issues, use this detailed reporting format:

```
COHERENCE ISSUE: [Short title of the issue]
- TYPE: [Contradiction | Gap | Ambiguity | Circularity]
- LOCATION: [Document A] <-> [Document B]
- DESCRIPTION: [Describe the issue]
- IMPACT: [What problems could this cause?]
- RESOLUTION OPTIONS:
  1. [Option 1]
  2. [Option 2]
```

---

## 🧠 Meta-Reflection

> If your system includes a Coherence Check… it also needs a check for the Coherence Check.

This protocol, along with [PROCESS_ARCHITECTURE.md](./PROCESS_ARCHITECTURE.md), forms the meta-coherence layer that ensures the overall system remains internally consistent even as it evolves.

---

## 📄 References
- [COHERENCE_CHECK.md](./COHERENCE_CHECK.md): Individual instance coherence validation
- [PROCESS_ARCHITECTURE.md](./PROCESS_ARCHITECTURE.md): Map of process relationships
- [VALIDATION.md](../VALIDATION.md): Documentation technical validation
- [MAP.md](../project/blueprint/MAP.md): Project dependency mappings