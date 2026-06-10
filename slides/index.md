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
- **not deterministic**

</div>

<div>

### **AI Agent**
- LLM + tools + specifications + memory
- MCP (tools): run python, search the web
- Skills (manuals and workflow)
- Role definitions ('agents' = identity)
- Various kinds of memory

</div>
</div>

<div class="box warning">
⚠️Agents can modify their own context: Choose skill, tool etc. New challenges for security.
</div>

---

## Context

<div class="cols">

<div>

### **Memory**

<div class="box">
Stored data with which context is augmented
</div>

- **procedural memory**: workflows, skills, rules, tools, system prompt, 'learned behavior'
- **episodic memory**: 'experiences', specific events, interactions, outcomes
- **semantic memory**: facts, entity relationships, scope definitions, weights, RAG
- **working memory**: The context window
    - current interaction
    - open files

</div>

<div>

### **Context**

<div class="box">

Not just what you write into the chat window.

</div>

- interaction history, including current prompt
- system prompt: General behavior, role definition, rules to always follow
    - Agent definitions can replace this with your own
- tool definitions, output and execution results
- chain of thought (in reasoning mode)
- Selected elements of memory
    - skill or subagent definitions
    - parts of episodic memory
    - facts or semantic memory

</div>
</div>

---

## Context engineering
- How to manipulate model context to make it effective and efficient
- What does the model see at any given point
- Automatically done by LLM/Agent vendor:
    - context summarization (automatically done): Can oversimplify
    - progressive disclosure of files, skills, tools...
    - when to write memory
    - system prompt
- Manually done by user:
    - fresh context window for new task
    - prompt engineering
    - when to clear context
---

## Agent Harness and harness engineering

<div class="box">

- **Harness**: Execution environment (operationg system) of the Agent
- **Harness engineering**: Designing the execution environment around an LLM

</div>

- Memory: Skills, subagents, Tools
- Workflow model and task progression
    - task progression and structuring
    - context engineering
    - human approval gates
    - feedback loops
- sandboxing
- security boundaries
- treat failure as a system problem, not a prompt to retry

<div class="box">

The harness is the dominant influence on quality, not the LLM!
TODO: references to corroborate this

</div>


<!-- ---
## Applications

- literature review
- summarization of results
- teaching and education (student and teacher)
- simple experiment loops:
    - evaluate - hypothesis - modify - evaluate - ...
- writing new skills for an agent
- drafting of text
- create illustrations
- coding -->

---
## Coding with AI Agents

- Cooperation between human and machine
- Scientific work is (typically) not in the training data
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
- Makes development a lot faster
- Great for debugging and tracing errors
- Great for processing a lot of 'stuff' quickly
    - finding and review literature
    - summarize results from 200 ML experiments
    - find libraries, read documentation, generate 'cookbooks'
- Good for larger projects or more diverse work...
    - ... if context and harness are engineered well
- Local focus: LLMs struggle with the big picture
    - Architecture, global requirements, ingrained assumptions...
    - Agents compensate for ignorance with complexity

---
## Our Experiences with (coding) agents
- Role change: Hands-on developer to Product owner/manager/architect/senior dev
    - Reviewing and permanent vigilence can become exhausting
    - Changes the daily workflow
- Deep understanding becomes more important more quickly:
    - Planning, requirements engineering
    - tests and constraints...
- Techniques that once were not practical now become feasible and beneficial
    - Code can get better through use of coding agents
- Use of coding agents might make larger projects more feasible
    - Transfer old code to new languages

---
### Spec-driven development
- Specifications of your intent are the source of truth
- Specifications are living elements of your project, just as much as code and tests are
- Specifications evolve together with you code and tests
- Specifications define desired behavior, behavior defines tests and acceptance criteria, tests define code

---
### Useful Software engineering techniques
- Behavior- driven development
    - facilitate structured communication between different team members (here: you + agent)
    - central concept: User story in structured natural language
    - derive automated test from user story, check if implemented code allows it
    - `pytest-bdd`, `behave`, `cucumber`
- Mutation testing
    - bottleneck: Which mutants are useful, and how to turn them into tests?
    - how sensitive is your test suite to code mutations?
    - generate mutant codes, run tests, surviving (uncaught) mutants are used to write better tests
    - helps with finding correctness or performance regressions, security compliance

---
## General best practices for agentic AI


---
### Security aspects
- zero trust principle
- progressive disclosure
- minimal priviledges

---

## Summary
TODO


---
## References
TODO