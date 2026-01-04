# Francesco Maiomascio

[![Buy Me a Coffee](https://img.shields.io/badge/Buy%20Me%20a%20Coffee-support-FFDD00?style=flat&logo=buy-me-a-coffee&logoColor=black)](https://buymeacoffee.com/francescomaiomascio)
[![GitHub Sponsors](https://img.shields.io/badge/support-GitHub%20Sponsors-7A7CFF?style=flat)](https://github.com/sponsors/francescomaiomascio)
[![ICE Docs](https://img.shields.io/badge/ICE%20Docs-8FB9FF?style=flat)](https://francescomaiomascio.github.io/ICE-Studio-Docs/)
[![Focus](https://img.shields.io/badge/focus-cognitive%20systems-111827?style=flat)](#)
[![Status](https://img.shields.io/badge/status-active%20research-6B7280?style=flat)](#)

I design and engineer **runtime-centric cognitive systems** and **AI execution architectures**
where intelligence is treated as a **controlled process**, not an implicit property of a model.

My work focuses on **orchestration, execution semantics, and system invariants**
for long-running, multi-agent, memory-bearing AI systems.

This is not applied prompt engineering.
This is **systems architecture**.

---

## Technical focus areas

- Cognitive runtimes and execution models  
- Event-sourced and event-derived systems  
- Deterministic run lifecycles (provision → execute → validate → commit)  
- Agent-based systems under strict runtime governance  
- Capability-based security and resource control  
- Structured memory models (event-derived, versioned, auditable)  
- Local-first and hybrid execution environments  

---

## ICE — Runtime Architecture Research

ICE is a **runtime specification and implementation effort**, not a framework.

It defines a **kernel-like execution environment** for cognitive systems, built around:

- explicit run lifecycles  
- event-only state derivation  
- post-hoc auditability without model replay  
- capability-gated side effects  
- memory as a promoted, governed artifact  

The core assumption is simple and non-negotiable:

> Models do inference.  
> Runtimes decide what is allowed to happen.

---

## Architectural characteristics

### Runtime-first execution

The runtime is the authority over:

- execution order  
- resource allocation  
- side effects  
- validation and commit  

Models and agents are treated as **inferential workers** operating inside
a constrained execution envelope.

There is no model-level authority.

---

### Event-derived state

ICE is an **event-only system**.

- No mutation occurs without an event  
- Events are append-only  
- State is always a projection  
- Replay is deterministic  

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

A Run always follows a fixed lifecycle:
provisioning → context loading → execution → validation → commit/abort → teardown.

There are no implicit transitions.

---

### Memory as a governed artifact

Memory is **not context** and **not model state**.

In ICE:
- memory is derived from validated events  
- promotion to memory is explicit  
- memory is typed, versioned, and policy-bound  
- memory can expire, degrade, or be invalidated  

Vector indices and embeddings are treated as **access structures**, not memory.

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

## Implementation scope

ICE is implemented as a **multi-repository system** covering:

- runtime core and orchestration  
- agent execution layers  
- memory and storage engines  
- protocol and transport layers  
- API and UI boundaries  
- test suites defined by contract, not behavior  

The codebase is intentionally modular to allow:
- subsystem replacement  
- controlled refactors  
- parallel evolution of components  

---

## ICE Studio

ICE Studio is a **reference environment** built on top of the ICE runtime.

It exists to:
- exercise the runtime under real workloads  
- validate architectural assumptions  
- expose failure modes early  

It is not the goal.
It is a testbed.

---

## Documentation

- Architecture notes, runtime specifications, and design documents  
  https://francescomaiomascio.github.io/ice-docs/

These documents are **engineering notes and RFC-style specifications**,
not tutorials or marketing material.

---

## Support

If you are interested in **runtime-level AI systems**,  
event-driven cognition, and long-term architectural research:

- Buy Me a Coffee  
  https://buymeacoffee.com/francescomaiomascio  

- GitHub Sponsors  
  https://github.com/sponsors/francescomaiomascio  

Support goes directly into sustained engineering work,
not short-term productization.
