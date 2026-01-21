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
  <strong>Inference</strong> produces <em>intent</em>. <strong>Execution</strong> is the responsibility to
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

I work on runtime architectures for AI-enabled systems, with a focus on
what happens after inference: when proposed actions become real, persistent state transitions.

Inference can produce intent, suggestions, or proposed actions.  
Execution is the phase where those proposals become real state transitions.
That transition is not automatic, and it is not neutral.

In practice, execution means deciding **who is allowed to act**, **when an action is legitimate**,
**how it changes system state**, and **how its effects can be observed, traced, and governed over time**.

The core problem is not intelligence itself.  
It is what happens *after* intelligence produces intent.

If an inference step proposes an action, what makes that action legitimate to execute?  
What authority enables it?  
What state is allowed to change?  
Where is responsibility located when things go wrong?

These questions are **architectural**, not algorithmic.

## How I turn execution theory into real systems

I build systems end-to-end, from execution semantics down to runtime behavior,
keeping control flow, state transitions, and side effects explicit in code.

I work primarily in Python, used as an execution and orchestration language.
Runtime logic is procedural and structured around:

- explicit pipelines
- state machines
- lifecycle phases
I deliberately avoid agent frameworks and high-level orchestration toolkits, preferring minimal building blocks where execution behavior stays visible.

State and persistence are handled explicitly through SQLite / SQL and DuckDB, used for execution state, checkpoints, and auditability. Where relational structure matters, I use SQLAlchemy selectively, without turning the system into an ORM-driven design.

For semantic indexing and retrieval, I work with sentence-transformers for embeddings and FAISS / Chroma for vector search, integrated as bounded components. Retrieval feeds execution logic but never bypasses validation or state rules.

Numerical validation and decision support rely on NumPy, SciPy, and scikit-learn for similarity, scoring, clustering, and thresholding. Machine learning supports execution decisions; it does not control them.

LLMs are used as inference components only. I primarily test open-source models via Hugging Face and local runtimes (e.g. ctransformers, LLaMA-based backends), treating model outputs as proposals that must pass explicit authority and state-transition checks.

At the systems level, I work directly with HTTP, WebSockets, and async I/O, and with filesystem and process signals where needed. Operational workflows are exposed through CLI/TUI tooling built with click, typer, and prompt_toolkit.

ICE is where this approach is currently exercised: an execution environment under active construction, used to validate ideas against real code, real state, and real failure modes.
 
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
