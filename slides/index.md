---
marp: true
theme: ssc
paginate: true
title: LLMs and Agentic AI in research
description: SSC workshop short constribution
---

<!-- _class: title -->
<!-- _paginate: false -->
<!-- _footer: "Last updated: 2026-05-26" -->


# LLMs and Agentic AI in research

## Liam Keegan, Harald Mack (SSC)

---
## LLMs and Agentic AI?

<div class="box warning">
⚠️LLMs and AI Agents are not the same!
</div>

<div class="cols">

<div>

### **LLM - 'Large language model'**
- process language piece by piece
- execution engine for agentic applications, similar to Python Interpreter vs App
- **stateless**: act only on current content of context window

</div>

<div>

### **AI Agent**
- LLM + tools + specifications
- Model
- MCP
- Skills

</div>
</div>

<div class="box warning">
⚠️Agents can modify their own context: Choose skill, tool etc. New challenges for security.
</div>

---

## Context

<div class="cols">

<div>

### **Prompt**

</div>
<div>

### **Memory**

</div>
</div>

---
## Agentic memory and Agent Harness

---
## Context engineering
How to manipulate model context to make it effective and efficient


---
## Applications

- literature review

- summarization of results

- simple experiment loops: evaluate - hypothesis - modify - evaluate - ...

- writing new skills for an agent

- coding

---
## Caveats of agentic applications


---
## Coding with AI Agents

- Cooperation between human and machine
- Science is (typically) not in the training data by definition
- Reversal of roles:
    - Machine knows more than we do about coding
    - Human is architect, product owner, carrier of responsibility, manager
- We need new skills or use existing ones in different ways:
    - how to express intent effectively
    - how to keep the agent on track
    - how to keep ourselves on track
    - software architecture, verification, validation

---
## Our Experiences with (coding) agents
- Great for debugging and tracing errors
- Great for processing a lot of 'stuff' quickly
    - finding and review literature
    - summarize results from 200 ML experiments
    - find libraries, read documentation, generate 'cookbooks'
- Good for larger projects or more diverse work...
    - ... if context and harness are engineered well for it
- Local focus: LLMs struggle with the big picture
    - Architecture, global requirements, ingrained assumptions...
    - Agents compensate for ignorance with complexity
- Deep understanding becomes more important more quickly:
    - Planning, requirements engineering, tests, boundary cases, constraints...
- Techniques that once were not practical now become feasible and beneficial
    - Code can get better through use of coding agents
- Role change: Hands-on developer to Product owner/manager/architect/senior dev
    - Reviewing and permanent vigilence can become exhausting

---
### Spec-driven development for 'intent engineering'
-


---
### Other useful agentic coding techniques
- Mutation testing
- Test-driven development
- Behavior- driven development
- Characterization tests (when migrating code bases)
-

---
### Security aspects
- zero trust principle
- progressive disclosure
- minimal priviledges

---
## Useful Agents (Harnesses)
- Claude
- Codex
- Cursor
- OpenClaw
- Pi (https://pi.dev/)
    - feynman


---

## Summary
TODO