# Francesco Maiomascio

[![ICE Documentation](https://img.shields.io/badge/ICE%20Docs-Architecture%20%26%20RFCs-8FB9FF?style=flat)](https://francescomaiomascio.github.io/ice-docs/)
[![Research Status](https://img.shields.io/badge/status-active%20research-6B7280?style=flat)](#)
[![GitHub Sponsors](https://img.shields.io/badge/support-GitHub%20Sponsors-7A7CFF?style=flat)](https://github.com/sponsors/francescomaiomascio)
[![Buy Me a Coffee](https://img.shields.io/badge/support-Buy%20Me%20a%20Coffee-FFDD00?style=flat&logo=buy-me-a-coffee&logoColor=black)](https://buymeacoffee.com/francescomaiomascio)

---

I work on the **design of execution environments for intelligent systems**.

My focus is not on models, prompts, or isolated AI capabilities.  
I am interested in how systems *run*:
how execution is structured, how state is produced, how effects are constrained,
and how long-running processes remain intelligible, auditable, and governable over time.

For me, intelligence is not something to showcase.  
It is something that must remain **operationally accountable**.

---

## Motivation

Most contemporary AI systems blur responsibility.

Decisions emerge from opaque interactions between models, memory, tools, and side effects.
State mutates implicitly.  
Effects propagate without clear authority.  

When something goes wrong, there is no single place where responsibility lives.

This is not only an AI problem.  
It is a systems problem.

As software increasingly mediates real-world decisions, the lack of explicit execution semantics,
lifecycle boundaries, and post-hoc auditability becomes a structural risk.

If intelligent systems are becoming infrastructure, then **execution must be governed as infrastructure**.

---

## Research orientation

My work explores how to design systems where:

- execution is explicit and policy-driven  
- state is derived, not implicitly mutated  
- side effects are capability-bound and traceable  
- memory is intentional, not accidental  
- long-running processes remain interpretable over time  

I approach this as **systems research**, not product engineering.

I care more about:
- invariants than features  
- lifecycles than demos  
- constraints than convenience  

Complexity is unavoidable.  
The problem is not to hide it, but to **structure it correctly**.

---

## ICE — Execution as a first-class concern

ICE (Intelligent Cognitive Ecosystem) is a **runtime architecture and research effort**.

It exists because the properties above cannot be reliably enforced inside
model-centric or framework-driven architectures.

ICE treats cognition as something that happens *inside* a governed execution environment,
not as an emergent property of models.

The core assumption is simple:

> Models perform inference.  
> Runtimes decide what is allowed to happen.

There is no model-level authority in ICE.

---

## Architectural principles

### Runtime sovereignty

The runtime is the authoritative component.

It controls:
- execution order  
- resource access  
- side effects  
- validation and commit  

Agents and models operate as inferential workers inside a constrained execution envelope.

---

### Event-derived state

ICE follows an **event-only model**.

- no implicit mutation  
- events are append-only  
- state is always a projection  
- replay is deterministic  

This applies uniformly to execution state, memory, capabilities, and domain effects.

---

### Explicit execution lifecycle

Every unit of work executes as a **Run**.

A Run is:
- isolated  
- finite  
- traceable  
- auditable  

Its lifecycle is explicit and invariant:

provision → context loading → execution → validation → commit or abort → teardown

There are no implicit transitions.

---

### Memory as a governed artifact

Memory is not context and not model state.

In ICE:
- memory is promoted from validated events  
- promotion is explicit  
- memory is typed, versioned, and policy-bound  
- memory can expire, degrade, or be invalidated  

Vector stores and embeddings are treated as access structures, not memory itself.

---

### Capability-based action model

No action is implicit.

All interactions with:
- filesystem  
- network  
- external APIs  
- domain operations  
- compute resources  

require explicit, revocable capabilities granted by the runtime.

Capability usage is fully event-traced.

---

## ICE Studio

ICE Studio is a **reference environment** built on top of the ICE runtime.

Its role is to:
- exercise the runtime under real workloads  
- validate architectural assumptions  
- expose failure modes early  

ICE Studio is not the goal.  
It is a **testbed**.

---

## Documentation

Architecture notes, runtime specifications, and design documents are available at:

https://francescomaiomascio.github.io/ice-docs/

These are engineering notes and RFC-style documents.  
They are written for people who already work on systems, not as tutorials or marketing material.

---

## Support

If you are interested in runtime-level AI systems,
event-derived cognition, and long-term architectural research:

- GitHub Sponsors  
  https://github.com/sponsors/francescomaiomascio  

- Buy Me a Coffee  
  https://buymeacoffee.com/francescomaiomascio  

Support goes directly into sustained engineering and research work,
not short-term productization.
