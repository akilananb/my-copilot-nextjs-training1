# Day 0 — VSCode & GitHub Copilot Deep Dive (Foundation Day)
## GenAI Spec-Driven Development Workshop

---

# Day 0 Goal

By the end of Day 0, participants will:

- Be fully comfortable navigating VSCode
- Understand the GitHub Copilot UI inside VSCode
- Understand:
  - Inline suggestions
  - Copilot Chat
  - Different chat modes
  - Context (current file, selection, workspace)
  - How Copilot reads your project
- Know how to:
  - Accept changes
  - Reject changes
  - Ask Copilot to refine
  - Ask Copilot to explain
- Understand the limits of AI and how to work with it safely
- Be ready to use AI productively on Day 1

---

# Who This Day Is For

- Product Owners
- Business Analysts
- Developers
- QA
- Architects

---

# Key Philosophy

> AI is not a brain.  
> AI is a very fast text generator that follows instructions.

> You are always responsible for correctness.

---

# Agenda

1. VSCode overview
2. VSCode layout and UI
3. Installing and enabling Copilot
4. Copilot inline suggestions
5. Copilot Chat window
6. Chat modes and what they mean
7. Context: how Copilot sees your project
8. Editing with Copilot: accept / reject / refine
9. Using Copilot for non-code tasks
10. Common mistakes and safety rules

---

# Module 0.1 — VSCode Overview

## What VSCode Is

VSCode is:

- A code editor
- A file explorer
- A terminal
- A Git client
- An AI workstation

Everything in this workshop happens inside VSCode.

---

# Module 0.2 — VSCode Layout

## Main Areas

- Left sidebar:
  - Explorer (files)
  - Search
  - Git
  - Extensions
- Center:
  - Editor (open files)
- Bottom:
  - Terminal
  - Output
  - Problems

## Exercise 0.2

- Open VSCode
- Open any folder
- Click:
  - Explorer
  - Search
  - Source Control
  - Extensions
- Open the terminal

---

# Module 0.3 — Installing and Enabling Copilot

## What You Need

- GitHub account
- Copilot enabled

## Exercise 0.3

- Open Extensions
- Search for "GitHub Copilot"
- Install it
- Sign in
- Verify Copilot icon appears in bottom bar

---

# Module 0.4 — Copilot Inline Suggestions

## What They Are

- As you type, Copilot shows grey "ghost text"
- This is a suggestion, not a command

## How To Control

- Press Tab → Accept
- Keep typing → Ignore
- Esc → Dismiss

## Exercise 0.4

- Create file: `demo.js`
- Type:

```
function multiply(a, b) {
```

- Observe suggestion
- Accept it
- Modify the function yourself

---

# Module 0.5 — Copilot Chat Window

## What It Is

Copilot Chat is:

- A conversation window with AI
- It can:
  - Answer questions
  - Explain code
  - Propose changes
  - Generate new code
  - Review code

## Where It Is

- Usually in the right sidebar or bottom panel

## Exercise 0.5

- Open Copilot Chat
- Ask:

```
What is this project about?
```

- Ask:

```
Explain what a JavaScript function is
```

---

# Module 0.6 — Chat Modes (Very Important)

## Different Ways to Talk to Copilot

Copilot Chat usually has modes like:

- Ask / Chat:
  - Just answer questions
- Edit:
  - Modify selected code
- Agent:
  - Perform bigger tasks across files

## Mental Model

- Ask → Talk
- Edit → Change this
- Agent → Do work

---

# Module 0.7 — Using Chat with Selection

## Very Important Concept

Copilot pays special attention to:

- The file you have open
- The text you have selected

## Exercise 0.7

- Select a function
- Ask in chat:

```
Explain this code
```

Then:

```
Refactor this to be more readable
```

Observe:

- It only touches the selected code

---

# Module 0.8 — Context: How Copilot Sees Your Project

## What Copilot Can See

- Current file
- Open files
- Sometimes other files in workspace
- Your selection
- Filenames and structure

## What It Cannot See

- Your brain
- Your unstated rules
- Your architecture decisions

## Key Rule

> If it is not in files or prompt, it does not exist.

---

# Module 0.9 — Using Copilot to Edit Code

## Typical Flow

1. Select code
2. Ask Copilot to change it
3. Copilot proposes a diff
4. You:
   - Accept
   - Reject
   - Ask to refine

## Exercise 0.9

- Ask Copilot:

```
Add input validation to this function
```

- Review proposed change
- Accept or reject it

---

# Module 0.10 — Accepting and Rejecting Changes

## Important Rule

> Never blindly accept.

Always:

- Read the change
- Check logic
- Check edge cases
- Check style

## Exercise 0.10

- Ask Copilot to make a change
- Intentionally:
  - Reject it
  - Then ask it to try again in a different way

---

# Module 0.11 — Using Copilot for Non-Code Work

## You Can Ask Copilot To

- Write documentation
- Summarize files
- Explain errors
- Generate test cases
- Draft requirements

## Exercise 0.11

Ask:

```
Write a README for this project
```

Then:

```
Make it shorter and more technical
```

---

# Module 0.12 — Common Mistakes

## Do NOT

- Blindly accept code
- Give vague instructions
- Assume Copilot understands your business
- Use Copilot without reading output

---

# Module 0.13 — Safety Rules

- You are responsible
- AI can be wrong
- Always review
- Always test
- Always think

---

# Module 0.14 — Preparation for Day 1

## Tomorrow You Will

- Use AI to analyze problems
- Generate epics and stories
- Draft specs

## What You Must Be Comfortable With

- VSCode UI
- Copilot Chat
- Selecting code
- Accepting/rejecting changes

---

# End of Day 0

## What You Should Now Believe

- Copilot is a powerful assistant, not an engineer
- Context controls quality
- Review is mandatory
- Tomorrow we use AI for real engineering thinking

---

> Day 0 builds comfort.  
> Day 1 builds brains.  
> Day 2 builds systems.
