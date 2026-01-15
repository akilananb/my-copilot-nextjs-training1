# Day 2 — From Specs to Working Software (OpenSpec Execution Day)
## GenAI Spec-Driven Development Workshop

---

# Day 2 Goal

By the end of Day 2, teams will:

- Start from the artifacts produced on Day 1 (stories, draft specs, architecture notes)
- Install and initialize OpenSpec in a repo
- Understand the OpenSpec folder structure
- Use OpenSpec commands to:
  - Create a change proposal
  - Review proposal, design, tasks, and spec diffs
  - Apply the change using AI
  - Archive the change
- Understand and customize:
  - copilot-instructions.md (how code must be written)
  - agents.md (how agents must think and work)
- Deliver a working demo with updated specs

---

# Key Philosophy

> Day 1 created intent.  
> Day 2 turns intent into software.

> We do not prompt for code.  
> We execute specs.

---

# Agenda

1. Mental model: AI as a junior team
2. Installing and initializing OpenSpec
3. Understanding the repo structure
4. Understanding copilot-instructions.md
5. Understanding agents.md
6. Preparing the spec from Day 1
7. Creating a change proposal
8. Reviewing before coding
9. Applying the change
10. Archiving and updating specs
11. Demo and retrospective

---

# Module 2.1 — Mental Model: AI as a Junior Team

## Explanation

When you use OpenSpec, you are not chatting.

You are orchestrating a workflow:

- A planner that reads specs
- A designer that proposes changes
- A task generator
- A code writer
- A reviewer

## Key Rule

> If instructions and specs are unclear, the "team" will fail.

---

# Module 2.2 — Install and Initialize OpenSpec

## Step 1: Install

In your project folder, run:

```
npm install -g openspec
```

Verify:

```
openspec --help
```

## Step 2: Initialize

Inside your project repo:

```
openspec init
```

This creates a new folder:

```
openspec/
```

---

# Module 2.3 — Understand the Folder Structure

After init, you will see:

```
openspec/
  project.md
  agents.md
  copilot-instructions.md
  specs/
  changes/
```

## What Each File Is

- project.md
  - High-level description of the system

- copilot-instructions.md
  - Rules for HOW code must be written

- agents.md
  - Rules for HOW work must be planned and executed

- specs/
  - The living specification of the system

- changes/
  - All ongoing and completed change proposals

---

# Module 2.4 — copilot-instructions.md (How to Code)

## What This File Controls

This file tells Copilot:

- Architecture rules
- Layering rules
- Error handling rules
- Testing rules
- Naming conventions
- Forbidden patterns

## Example Rules

- No business logic in controllers
- Always validate input
- Always write tests for new logic
- Use service layer for business logic

## Exercise 2.4

- Open copilot-instructions.md
- Read it
- Add 5 rules that match your team standards

---

# Module 2.5 — agents.md (How to Think and Work)

## What This File Controls

This file tells agents:

- What must be read before coding
- How to break work into tasks
- What must never be skipped
- What must be updated after work

## Example Rules

- Always read relevant specs before coding
- Never modify files not listed in tasks
- Always update specs after change
- Prefer small, verifiable tasks

## Exercise 2.5

- Open agents.md
- Read the checklist
- Add 5 process rules for your team

---

# Module 2.6 — Prepare Your Spec from Day 1

## What You Should Have

From Day 1:

- A story
- A draft spec
- Rules and constraints

## Exercise 2.6

- Pick ONE story
- Convert its spec into a clean, precise spec file under:

```
openspec/specs/<your-area>/spec.md
```

- Make sure it contains:
  - Behaviors
  - Rules
  - Edge cases
  - Non-goals

---

# Module 2.7 — Our Running Example

We will use:

> "Add Remember Me to Login (30 day session)"

Rules:

- If checked → session expires in 30 days
- If not checked → session expires in 30 minutes
- Logout invalidates all sessions
- Password change invalidates all sessions

---

# Module 2.8 — Create a Change Proposal

## Command

```
openspec proposal "Add Remember Me to Login"
```

(or in Copilot Chat)

```
/openspec:proposal Add Remember Me to Login
```

## What OpenSpec Does

- Reads current specs
- Reads code
- Generates a new folder:

```
openspec/changes/add-remember-me/
  proposal.md
  design.md
  tasks.md
  specs/
```

---

# Module 2.9 — Understand the Generated Files

## proposal.md

- Human-readable explanation of the change
- Why it exists
- What will change

## design.md

- Technical approach
- Architecture decisions
- Tradeoffs

## tasks.md

- Step-by-step implementation plan
- What files to touch
- In what order

## specs/

- Shows the exact spec changes

---

# Module 2.10 — Review Before Coding (Most Important Step)

## Why

> If spec or tasks are wrong, code will be wrong.

## Review Checklist

- Are rules missing?
- Are edge cases missing?
- Are tasks too big?
- Are tasks unclear?
- Any wrong assumptions?

## Exercise 2.10

- Edit:
  - proposal.md
  - design.md
  - tasks.md
  - spec files
- Do NOT write code yet

---

# Module 2.11 — Apply the Change

## Command

```
openspec apply add-remember-me
```

(or)

```
/openspec:apply add-remember-me
```

## What Happens

- Agent executes tasks
- Copilot writes code
- Files are modified
- Tests may be added

## Exercise 2.11

- Apply the change
- Review the code
- Run the app or tests
- Fix obvious issues

---

# Module 2.12 — Archive the Change

## Command

```
openspec archive add-remember-me
```

## What This Does

- Merges spec changes into main specs
- Marks change as completed
- Preserves knowledge permanently

## Exercise 2.12

- Archive the change
- Review:

```
openspec/specs/
```

- Confirm your feature is now documented

---

# Module 2.13 — Full Team Demo

Each team presents:

- Their story
- Their spec
- Their proposal and tasks
- Their copilot-instructions.md rules
- Their agents.md rules
- Their working feature

---

# Module 2.14 — Retrospective

Discuss:

- Where did specs save you?
- Where did AI help?
- Where did AI fail?
- Where would vibe coding have failed?
- What rules will you add next time?

---

# The New Development Model

Old:

Story → Prompt → Code → Debug → Patch

New:

Story → Spec → Proposal → Review → Apply → Updated Spec

---

# Final Lessons

- You must govern AI, not just use it
- Specs define what to build
- Instructions define how to build
- Agents define how to think
- This is how teams scale AI safely

---

# End of Day 2

> You are no longer prompting.  
> You are running an AI-powered engineering process.
