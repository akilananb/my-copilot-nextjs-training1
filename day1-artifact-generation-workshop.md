# Day 1 — Using AI to Think, Analyze, and Design (Artifact Generation Day)
## GenAI Spec-Driven Development Workshop

---

# Day 1 Goal

By the end of Day 1, teams will:

- Stop using AI only for writing code
- Learn to use AI for:
  - Requirement analysis
  - Architecture review
  - Risk analysis
  - Epic generation
  - Story generation
  - Spec drafting
- Learn prompting techniques AND what they mean
- Apply those techniques to generate real artifacts
- Produce real outputs that will be used on Day 2

---

# What We Will Produce Today

Each team will leave Day 1 with:

- A chosen domain & problem
- A clarified problem statement
- A list of business rules and constraints
- A rough architecture
- A set of epics
- A set of stories
- A first draft spec per story

---

# Key Philosophy

> AI is not a coding tool.  
> AI is a thinking, analysis, and design accelerator.

---

# Agenda

1. Pick domain & problem
2. Use AI to analyze requirements (Zero-shot, Role, Chain-of-thought)
3. Use AI to review architecture
4. Use AI to generate epics and stories (Few-shot, Context injection)
5. Use AI to draft specs (Structured prompting)
6. Package outputs for Day 2

---

# Module 1.1 — Pick Your Domain and Problem

## Instructions

Each team chooses:

- Any domain (banking, SaaS, internal system, workflow, reporting)
- One core problem area (auth, approval, payment, onboarding, etc.)

## Rules

- Must be realistic
- Must have rules
- Must have edge cases
- Must not be too big

## Exercise 1.1

- Pick domain
- Write 1-paragraph problem statement

---

# Module 1.2 — Zero-Shot Prompting (Baseline Thinking)

## What It Is

Zero-shot means:

- You give the AI only an instruction
- No examples
- No structure
- No guidance

The AI must guess everything.

## Why It Is Useful

- To see what the AI assumes
- To expose ambiguity in your problem
- To discover hidden requirements

## Exercise 1.2

Ask AI:

"Analyze this problem domain and list major requirements and risks."

Observe:

- What did it assume?
- What did it miss?
- What is vague?

---

# Module 1.3 — Role Prompting (Expert Thinking)

## What It Is

You tell the AI who it should act as:

- Senior architect
- Security reviewer
- Domain expert
- Product owner

This changes:

- What it focuses on
- How strict it is
- What risks it sees

## Exercise 1.3

Ask AI:

"You are a senior architect. Review this problem and list major components and risks."

Then:

"You are a security engineer. Review this problem and list security risks."

Compare outputs.

---

# Module 1.4 — Chain-of-Thought Prompting (Deep Reasoning)

## What It Is

You force the AI to:

- Think step by step
- Explain reasoning
- Not jump to conclusions

## When It Is Useful

- User journeys
- Business rules
- Multi-step logic
- Failure scenarios

## Exercise 1.4

Ask AI:

"Think step by step and explain how a user goes through this system and where it can fail."

---

# Module 1.5 — Meta Prompting (Improving Your Questions)

## What It Is

You ask AI to:

- Rewrite your prompt
- Make it more precise
- Make it more complete

## Why It Matters

- Most bad results come from bad prompts
- This technique fixes that

## Exercise 1.5

- Take your worst prompt so far
- Ask AI: "Improve this prompt to be more precise"
- Use improved prompt and compare output

---

# Module 1.6 — Few-Shot Prompting (Teaching by Example)

## What It Is

You give:

- 2–5 examples
- The AI copies the pattern

## When It Is Useful

- Classification
- Formatting
- Structured outputs
- Consistent style

## Exercise 1.6

Give AI examples of good stories and ask it to generate more stories in the same style.

---

# Module 1.7 — Context Injection / RAG (Giving AI Memory)

## What It Is

You paste:

- Rules
- Constraints
- Decisions
- Architecture

Into the prompt.

Now the AI:

- Does not need to guess
- Does not need to remember

## Exercise 1.7

- Generate stories without context
- Then generate again WITH full context
- Compare quality

---

# Module 1.8 — Generate High-Level Architecture

## Prompt Pattern

"Given these requirements and constraints, propose a simple architecture."

Then:

"Critique this architecture and find weaknesses."

## Exercise 1.8

- Generate architecture
- Let AI review its own architecture

---

# Module 1.9 — Generate Epics

## What Is an Epic

- A large business capability
- Groups multiple stories

## Prompt Pattern

"Based on this problem and architecture, generate epics."

## Exercise 1.9

- Generate 5–10 epics
- Merge and simplify

---

# Module 1.10 — Generate Stories

## Prompt Pattern

"Break this epic into implementable user stories with acceptance criteria."

## Exercise 1.10

- Generate stories per epic
- Ask AI: "What stories are missing?"

---

# Module 1.11 — Draft Specs from Stories

## What Is a Spec

A spec describes:

- Behaviors
- Rules
- Constraints
- Edge cases
- Non-goals

## Prompt Pattern

"Convert this story into a formal spec."

## Exercise 1.11

- Pick 1 story
- Generate spec draft
- Review precision and testability

---

# Module 1.12 — Spec Review (Critical Thinking)

## Prompt Pattern

"Review this spec like a strict reviewer and find gaps and ambiguities."

## Exercise 1.12

- Let AI criticize the spec
- Fix it
- Repeat once

---

# Module 1.13 — Package Artifacts for Day 2

## What You Must Have

Each team must have:

- Problem statement
- Architecture summary
- Epics list
- Stories list
- At least 1 good spec

## Exercise 1.13

- Save all artifacts into files
- Commit them
- These become OpenSpec inputs tomorrow

---

# End of Day 1

## What You Should Now Believe

- Prompting is a design skill
- AI is a thinking partner
- Specs are the real output
- Tomorrow we turn intent into code

---

> Day 1 builds the brain.  
> Day 2 builds the system.
