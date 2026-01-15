# GenAI Spec-Driven Development Workshop
## Using VSCode, GitHub Copilot, and OpenSpec

---

# Workshop Goal

By the end of this workshop, participants will:

- Understand how to use AI safely for software development
- Understand why "vibe coding" fails
- Learn structured prompting
- Learn spec-driven development
- Use OpenSpec to deliver a feature end-to-end
- Build a working demo from story → spec → code → test

---

# Workshop Structure

- Day 0: Absolute Beginners (PO / Non-technical)
- Day 1: Developers (Prompting + Spec Thinking)
- Day 2: Developers (OpenSpec + End-to-End Delivery)

---

# DAY 0 — AI & VSCode BASICS

## Module 0.1 — What is VSCode?

### Topics
- What is an editor
- Files and folders
- Opening a project
- Editing files
- Terminal inside VSCode
- Extensions

### Exercise 0.1
- Open VSCode
- Create a folder called `demo-app`
- Create a file called `README.md`
- Write 3 lines of text
- Open terminal inside VSCode

---

## Module 0.2 — What is GitHub Copilot?

### Topics
- What Copilot is
- Inline suggestions
- Copilot chat
- Accepting / rejecting suggestions

### Exercise 0.2
- Create `hello.js`
- Type: `function add(a, b) {`
- Accept Copilot suggestion
- Ask Copilot Chat: "Explain this function in simple words"

---

## Module 0.3 — AI is Not Magic

### Topics
- AI predicts text
- AI does not understand business
- AI follows instructions literally
- Bad instructions = bad output

### Exercise 0.3
Ask Copilot:
Build a login system

Discuss:
- What did it assume?
- What is missing?
- What is unclear?

---

# DAY 1 — PROMPTING & SPECS

## Module 1.1 — The Vibe Coding Problem

### Topics
- Vague prompts
- Guessing requirements
- Hidden assumptions
- Context window problem

### Exercise 1.1
Ask Copilot:
Build a photo album feature

List:
- What decisions did AI guess?
- What questions should have been asked?

---

## Module 1.2 — Zero-Shot Prompting

### Topics
- No examples
- Just instruction
- High ambiguity

### Exercise 1.2
Prompt:
Write a function to validate email

Discuss:
- What rules did it assume?
- What is missing?

---

## Module 1.3 — One-Shot and Few-Shot Prompting

### Topics
- Showing examples
- Teaching pattern by example

### Exercise 1.3
Prompt examples:
"3" -> odd
"10" -> even
"7" ->

Observe:
- How example changes output

---

## Module 1.4 — Role Prompting

### Topics
- Assigning persona
- Changes tone and quality

### Exercise 1.4
Compare:
Design a login API
vs
You are a senior backend engineer. Design a login API.

---

## Module 1.5 — Chain of Thought

### Topics
- Forcing step-by-step thinking
- Reduces logical errors

### Exercise 1.5
Prompt:
Explain step by step how password validation should work

---

## Module 1.6 — ReAct Prompting

### Topics
- Think → Act → Observe → Answer
- Used for multi-step reasoning

### Exercise 1.6
Ask:
Find what fields a login API needs and explain your reasoning

---

## Module 1.7 — Meta Prompting

### Topics
- AI improves your prompt

### Exercise 1.7
Prompt:
Improve this prompt: "Build a login feature"

---

## Module 1.8 — RAG / Context Prompting

### Topics
- Injecting rules and documents
- Context beats memory

### Exercise 1.8
Give Copilot:
Here is our rule: Password must be at least 12 chars. Now generate validation code.

---

## Module 1.9 — Why Prompting Is Not Enough

### Topics
- Prompts are not persistent
- Prompts are not reviewed
- Prompts are not shared
- We need specs

---

## Module 1.10 — What is a Spec?

### Topics
- Describes behavior
- Describes rules
- Describes non-goals
- Describes acceptance criteria

### Exercise 1.10
Write a spec for:
User can login

Include:
- Valid cases
- Invalid cases
- Rules

---

# DAY 2 — OPENSPEC WORKFLOW

## Module 2.1 — What is OpenSpec?

### Topics
- Specs live in repo
- Specs drive implementation
- AI reads specs
- Specs survive time

---

## Module 2.2 — OpenSpec Project Setup

### Exercise 2.2
- Initialize OpenSpec in project
- Explore folders
- Read project spec file

---

## Module 2.3 — Creating a Change Proposal

### Topics
- From story to spec change
- From spec change to tasks

### Exercise 2.3
Create a proposal for:
Add Remember Me to Login

Review:
- Proposal
- Design
- Task list

---

## Module 2.4 — Reviewing Before Coding

### Topics
- Review spec
- Review tasks
- Fix mistakes BEFORE code exists

### Exercise 2.4
- Improve generated tasks
- Fix missing cases

---

## Module 2.5 — Applying the Change

### Exercise 2.5
- Apply the change
- Let Copilot implement code
- Run the app/tests

---

## Module 2.6 — Archiving the Change

### Topics
- Spec becomes source of truth
- Change is now permanent knowledge

### Exercise 2.6
- Archive the change
- Review updated spec

---

## Module 2.7 — Full End-to-End Flow

### Final Exercise
Teams must:
1. Pick a small feature
2. Write spec
3. Create proposal
4. Review tasks
5. Apply change
6. Demo working feature
7. Show updated spec

---

# Final Principles

- AI is not intelligent, it is obedient
- Vague input creates vague systems
- Specs are context
- Context is power
- Spec-driven development is how you scale AI safely

---

# Final Message

If you don't design the system, the AI will.
