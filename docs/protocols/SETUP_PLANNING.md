# SETUP\_PLANNING.md

## 🧭 Purpose

This file is a guide for the **human initiator** of a project to collaboratively define the initial architecture, goals, and constraints with the help of an AI agent. The purpose is to:

* Establish foundational direction and design clarity
* Set up the relevant project documentation
* Enable long stretches of autonomous AI development without misalignment

---

## 🔄 Setup Process Overview

### Step 1: Initiate Conversation with AI

Start by opening a planning session with the AI. Prompt it to assist you in working through this file section-by-section.

### Step 2: Collaboratively Answer the Planning Prompts

The human and AI should work through the following prompts together. As answers stabilize, the AI should begin populating the corresponding documents.

### Step 3: Review and Revise

The human reviews all generated files. If something feels off:

* Ask the AI to rephrase, revise, or redesign
* Capture potential risks or confusion in `SCRATCH.md`

### Step 4: Sign Off and Begin Iteration

Once the initial setup is accepted by both agents:

* Lock in the structure
* Begin development using `cycle_development_process.md`

---

## 🧠 Key Prompts to Discuss

### 1. What Are We Building?

> Natural language description of what the project does, who it's for, and why it matters.

### 2. Goals and Constraints

> Define the project’s core values, priorities, and hard limitations.
> Populate → `PROJECT_SPECS.md`

### 3. High-Level Architecture

> Sketch an ideal layout: components, flows, domains, state models.
> Populate → `COMPONENT_ARCHITECTURE.md`

### 4. Implementation Plan

> Define initial features, dependencies, or tech stack decisions.
> Populate → `IMPLEMENTATION_PLAN.md`

### 5. Dev Philosophy & Division of Labor

> Clarify how AI and Human will collaborate.
> Populate → `HUMAN_AI_COLLABORATION.md`

### 6. Coding Strategy

> Discuss paradigms, file structures, naming standards.
> Reference → `AI_GUIDANCE.md`, `ARCHITECTURE_PATTERNS.md`

---

## 📄 Expected Output Files

* `project/identity/PROJECT_SPECS.md`
* `project/identity/HUMAN_AI_COLLABORATION.md`
* `project/identity/DESIGN_DECISIONS.md`
* `project/workspace/IMPLEMENTATION_PLAN.md`
* `project/workspace/COMPONENT_ARCHITECTURE.md`
* `project/workspace/DEVELOPMENT_LOG.md`
* `project/workspace/SCRATCH.md`

---

## ✅ Completion Criteria

* All prompts answered
* All docs generated and reviewed
* Human signs off with "Initial Setup Approved" in `DEVELOPMENT_LOG.md`

---

## 🔄 Navigation

* After setup, begin [cycle\_development\_process.md](../protocols/CYCLE_DEVELOPMENT_PROCESS.md)


> 🔁 For guidance on maintaining consistency across the project structure, see [COHERENCE_CHECK.md](./COHERENCE_CHECK.md) and [MAP.md](../project/blueprint/MAP.md).
