# Francesco Maiomascio

[![ICE Documentation](https://img.shields.io/badge/ICE%20Docs-Architecture%20%26%20RFCs-8FB9FF?style=flat)](https://francescomaiomascio.github.io/ice-docs/)
[![Research Status](https://img.shields.io/badge/status-active%20research-6B7280?style=flat)](#)
[![GitHub Sponsors](https://img.shields.io/badge/support-GitHub%20Sponsors-7A7CFF?style=flat)](https://github.com/sponsors/francescomaiomascio)
[![Buy Me a Coffee](https://img.shields.io/badge/support-Buy%20Me%20a%20Coffee-FFDD00?style=flat&logo=buy-me-a-coffee&logoColor=black)](https://buymeacoffee.com/francescomaiomascio)

---

## Who I am and what I work on

I design and study **execution-centric software systems**.

My work sits at the intersection of:
- runtime architecture  
- long-running process design  
- cognitive and agent-based systems  
- execution governance and observability  

I am not primarily interested in models, prompts, or isolated AI capabilities.
Those are components.

My focus is on the **environment in which intelligence executes**:
how computation is staged,
how state is produced and constrained,
how effects are validated,
and how a system remains understandable months or years after it started running.

I approach this as **systems work**, not as product development or AI experimentation.

---

## Why execution matters

Most contemporary intelligent systems are built around inference engines
and extended with tools, memory, and orchestration layers.

In practice, this leads to systems where:
- decisions emerge without explicit authority  
- state mutates implicitly across layers  
- side effects escape the scope in which they were produced  
- responsibility is diffused across components  

When something fails, it is often impossible to answer a simple question:
**why was this allowed to happen?**

This is not a limitation of intelligence.
It is a limitation of execution.

As intelligent systems increasingly operate as infrastructure,
execution semantics, lifecycle boundaries, and auditability
become first-class concerns.

---

## Research direction

My research explores how to design systems where:

- execution is explicit, staged, and governed  
- state is derived from validated events, not mutated implicitly  
- side effects are capability-scoped and observable  
- memory is a managed artifact, not an accidental residue  
- long-running processes remain intelligible over time  

This work is concerned with **structure**, not optimization.
With **control**, not performance benchmarks.
With **longevity**, not short-lived demos.

---

## ICE — Intelligent Cognitive Ecosystem

ICE is a **runtime architecture and research effort**.

It is not a framework and not a model.
It is an attempt to define a coherent execution environment
for cognitive and agent-based systems.

ICE starts from a simple but strict separation of concerns:

> Models produce suggestions.  
> Runtimes decide what actually happens.

In ICE, authority does not live at the model level.
It lives in the runtime.

---

## Core architectural ideas

### Execution as a governed process

ICE treats execution as a first-class entity.

Every unit of work runs inside an explicit **Run**:
- isolated  
- finite  
- traceable  
- auditable  

A Run follows a fixed lifecycle:
provision → context loading → execution → validation → commit or abort → teardown

There are no implicit transitions.

---

### Event-derived state

ICE follows an event-only model.

- no implicit mutation  
- events are append-only  
- state is always a projection  
- replay is deterministic  

This applies uniformly to execution state, memory, capabilities, and domain effects.

The system never asks *what is the state now?*  
It asks *which events led us here?*

---

### Capability-based effects

No operation is implicit.

All interactions with:
- filesystem  
- network  
- external services  
- domain-specific effects  

require explicit, revocable capabilities granted by the runtime.

Capability usage is event-traced and auditable by design.

---

### Memory as an explicit artifact

Memory is not context and not model state.

In ICE:
- memory is promoted from validated execution events  
- promotion is explicit and policy-driven  
- memory is typed, versioned, and degradable over time  

Vector stores and embeddings are treated as access mechanisms,
not as authoritative memory.

---

## ICE Studio — a user-facing environment

ICE Studio is a **reference application built on top of the ICE runtime**.

Its purpose is not to be an IDE replacement,
but an environment where users can:

- design and execute complex workflows  
- reason about long-running processes  
- develop and maintain code with execution awareness  
- observe system behavior over time  
- work with agents without delegating authority  

ICE Studio exists to validate ICE under real usage,
expose design flaws,
and explore how humans interact with governed cognitive systems.

It is an application.
ICE is the foundation beneath it.

---

## Documentation and materials

Architecture notes, runtime specifications, and design documents are available at:

https://francescomaiomascio.github.io/ice-docs/

These documents are written as engineering notes and RFC-style material.
They assume familiarity with systems, runtimes, and software architecture.

They are not tutorials.

---

## Support

This work is independent and long-term.

If you are interested in execution-centric AI systems,
runtime governance,
and the design of intelligible cognitive infrastructure:

- GitHub Sponsors  
  https://github.com/sponsors/francescomaiomascio  

- Buy Me a Coffee  
  https://buymeacoffee.com/francescomaiomascio  

Support goes directly into sustained research and engineering work,
not short-term productization.
