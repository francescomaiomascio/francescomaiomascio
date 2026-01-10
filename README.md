# Francesco Maiomascio

[![ICE Documentation](https://img.shields.io/badge/ICE%20Docs-Architecture%20%26%20RFCs-8FB9FF?style=flat)](https://francescomaiomascio.github.io/ice-docs/)
[![Research Status](https://img.shields.io/badge/status-active%20research-6B7280?style=flat)](#)
[![GitHub Sponsors](https://img.shields.io/badge/support-GitHub%20Sponsors-7A7CFF?style=flat)](https://github.com/sponsors/francescomaiomascio)
[![Buy Me a Coffee](https://img.shields.io/badge/support-Buy%20Me%20a%20Coffee-FFDD00?style=flat&logo=buy-me-a-coffee&logoColor=black)](https://buymeacoffee.com/fmaiomascio)

---

I design and engineer **runtime-centric cognitive systems**.

I am not primarily interested in models, prompts, or isolated AI capabilities.  
I am interested in **how intelligent systems execute**, how they are constrained, how they evolve over time, and how their effects can be observed, audited, and governed.

For me, intelligence is not an emergent property to be admired.  
It is a **process to be controlled**.

---

## Why this work exists

Most contemporary AI systems operate without a clear notion of authority.

Models decide.  
Side effects happen.  
State mutates.  
Memory accumulates.  

But no component is truly responsible for *why* something was allowed to happen.

This is not only an AI problem.

As software systems increasingly mediate real-world decisions, the absence of
explicit execution semantics, lifecycle governance, and post-hoc auditability
becomes a structural risk for the entire system we live in.

If intelligence is becoming infrastructural, then **execution must be sovereign**.

---

## My research focus

My work explores how to design systems where:

- execution is explicit and governed  
- state is derived, never mutated implicitly  
- side effects are capability-gated and traceable  
- memory is an artifact, not an accident  
- long-running processes remain intelligible over time  

I approach this as **systems research**, not product development.

I am interested in:
- invariants, not features  
- lifecycles, not demos  
- constraints, not convenience  

Complexity is not something to hide.  
It is something to **structure**.

---

## ICE — A runtime architecture, not a framework

ICE is a **runtime specification and implementation effort**.

It exists because the assumptions above cannot be validated inside traditional
model-centric or framework-driven architectures.

ICE defines a **kernel-like execution environment for cognitive systems**, built around:

- explicit run lifecycles  
- event-only state derivation  
- deterministic replay without model re-execution  
- capability-based control of side effects  
- memory derived from validated events  

The core assumption is simple and non-negotiable:

> Models perform inference.  
> Runtimes decide what is allowed to happen.

There is no model-level authority in ICE.

---

## Architectural characteristics

### Runtime-first execution

The runtime is the sovereign component.

It controls:
- execution order  
- resource allocation  
- side effects  
- validation and commit  

Agents and models operate as **inferential workers** inside a constrained execution envelope.

---

### Event-derived state

ICE is an **event-only system**.

- no mutation without an event  
- events are append-only  
- state is always a projection  
- replay is deterministic  

This applies uniformly to:
- execution state  
- memory  
- capabilities  
- domain effects  

---

### Explicit run lifecycle

Every unit of work executes as a **Run**:

- isolated  
- finite  
- traceable  
- auditable  

A Run follows a fixed lifecycle:

provision → context loading → execution → validation → commit or abort → teardown

No implicit transitions exist.

---

### Memory as a governed artifact

Memory is **not context** and **not model state**.

In ICE:
- memory is promoted from validated events  
- promotion is explicit  
- memory is typed, versioned, and policy-bound  
- memory can expire, degrade, or be invalidated  

Vector stores and embeddings are treated as **access structures**, not memory itself.

---

### Capability-based action model

No action is implicit.

All interactions with:
- filesystem  
- network  
- APIs  
- domain operations  
- compute resources  

require explicit, revocable **capabilities** granted by the runtime.

Capability usage is fully event-traced.

---

## ICE Studio

ICE Studio is a **reference environment** built on top of the ICE runtime.

It exists to:
- exercise the runtime under real workloads  
- validate architectural assumptions  
- expose failure modes early  

It is not the goal.  
It is a **testbed**.

---

## Documentation and research material

Architecture notes, runtime specifications, and design documents are available at:

https://francescomaiomascio.github.io/ice-docs/

These are **engineering notes and RFC-style documents**, not tutorials or marketing material.

They are written for people who already understand systems.

---

## Support

If you are interested in **runtime-level AI systems**,  
event-derived cognition, and long-term architectural research:

- GitHub Sponsors  
  https://github.com/sponsors/francescomaiomascio  

- Buy Me a Coffee  
  https://buymeacoffee.com/francescomaiomascio  

Support goes directly into sustained engineering work,  
not short-term productization.
