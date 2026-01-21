<!-- GITHUB STATUS / SIGNALS -->
<p align="center">
  <img src="https://img.shields.io/github/stars/francescomaiomascio/ice-runtime?label=stars&style=flat&labelColor=0b1220&color=7c3aed" />
  <img src="https://img.shields.io/github/issues/francescomaiomascio/ice-runtime?label=issues%20open&style=flat&labelColor=0b1220&color=10b981" />
  <img src="https://img.shields.io/github/last-commit/francescomaiomascio/ice-runtime?label=last%20commit&style=flat&labelColor=0b1220&color=6366f1" />
  <img src="https://img.shields.io/github/commit-activity/m/francescomaiomascio/ice-runtime?label=commit%20activity&style=flat&labelColor=0b1220&color=06b6d4" />
  <img src="https://img.shields.io/github/issues-pr/francescomaiomascio/ice-runtime?label=pull%20requests&style=flat&labelColor=0b1220&color=14b8a6" />
</p>

<!-- MANIFESTO / AXIOMS -->
<p align="center">
  <img
    src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&size=18&pause=1400&center=true&vCenter=true&width=640&lines=Running+intelligence%2C+beyond+inference.;Authority+precedes+execution.;Inference+is+not+control.;Traceability+is+structural."
  />
</p>



<p align="center">
  <strong>Inference</strong> produces <em>intent</em>.<br/>
  <strong>Execution</strong> is the responsibility to
</p>

<p align="center">
  <strong>authorize</strong> · <strong>execute</strong> ·
  <strong>observe</strong> · <strong>govern</strong><br/>
  <em>long-running, stateful systems</em>
</p>

<p align="center">
  Execution is an <strong>architectural primitive</strong>,
  not an implementation detail.
</p>


## What I work on

I work on **runtime architectures for AI-enabled systems**.

My interest is not centered on models, prompts, or inference quality in isolation.
What I focus on is what happens *after* inference, when intelligent systems are
expected to act in the world, persist over time, and remain accountable for their effects.

Inference can produce intent, suggestions, or proposed actions.  
Execution is the phase where those proposals become real state transitions.
That transition is not automatic, and it is not neutral.

In practice, execution means deciding **who is allowed to act**, **when an action is legitimate**,
**how it changes system state**, and **how its effects can be observed, traced, and governed over time**.
In long-running, stateful systems, these questions are not implementation details —
they define the system’s behavior.

Most AI systems implicitly assume that execution is obvious, delegated,
or safely handled by surrounding infrastructure.
This assumption may hold for prototypes, demos, or isolated tasks.
It breaks down as soon as systems are expected to run continuously,
interact with external environments, and remain accountable under real operational conditions.

The core problem is not intelligence itself.  
It is what happens *after* intelligence produces intent.

If an inference step proposes an action, what makes that action legitimate to execute?  
What authority enables it?  
What state is allowed to change?  
Where is responsibility located when things go wrong?

These questions are **architectural**, not algorithmic.


## How I turn execution theory into real systems


To explore execution as an architectural problem, I work on systems end-to-end,
from conceptual constraints down to concrete runtime behavior.

I tend to avoid large, opinionated frameworks whenever possible.
Instead, I prefer to build minimal execution layers from first principles,
so that authority, state transitions, and side effects are explicit in the code
rather than hidden behind abstractions.

Most of my work is implemented in **Python** for orchestration and system glue,
combined with **lower-level components** where determinism, isolation, or
performance matter. The goal is not performance at all costs, but *inspectability*:
being able to trace why a system acted, when it acted, and under which authority.

ICE (Intelligent Cognitive Ecosystem) is the environment where this work happens.
I use it as a controlled sandbox to experiment with execution models, lifecycle
boundaries, and runtime governance, rather than as a general-purpose framework.
Concepts are validated by being implemented, exercised, and broken under real
execution conditions.

On the engineering side, I treat **design rationale as part of the system**.
Work is organized around explicit issues, scoped changes, and reviewable pull
requests. Branches are short-lived, changes are intentional, and conceptual
decisions are recorded alongside code, not after the fact.

This approach lets me iterate simultaneously on:
- execution semantics
- runtime structure
- and the developer workflow that supports them

The result is not a polished product, but a continuously evolving execution
laboratory where ideas are tested against reality.


<p align="center">
  <em>Built with precision. Run with confidence.</em>
</p>

<p align="center">
  <img src="https://skillicons.dev/icons?i=python,rust,linux,git,github,docker,pytorch&theme=dark" />
</p>

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=francescomaiomascio&show_icons=false&theme=transparent&hide_title=true&hide_border=true&count_private=true" />
</p>

<p align="center">
  <img
    src="https://capsule-render.vercel.app/api?type=rect&height=2&color=0:0b2533,50:0891b2,100:0b2533&section=header"
    width="640"
  />
</p>


<p align="center">
  <img
    src="https://github-readme-activity-graph.vercel.app/graph?username=francescomaiomascio&theme=react-dark&hide_border=true&hide_title=true"
    width="78%"
  />
</p>




<p align="center" style="font-size: 0.9em; color: #9ca3af; max-width: 640px; margin: 0 auto;">
  This work is long-term, structural, and research-driven.
  If it proves valuable, its continuation can be supported.
</p>

<p align="center" style="margin-top: 12px;">
  <a href="https://www.buymeacoffee.com/francescomaiomascio">
    <img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" height="30" />
  </a>
</p>
