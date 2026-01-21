<!-- GITHUB STATUS / SIGNALS -->
<p align="center">
  <img src="https://img.shields.io/github/stars/francescomaiomascio/ice-runtime?label=stars&style=flat&labelColor=0b1220&color=a78bfa" />
  <img src="https://img.shields.io/github/issues/francescomaiomascio/ice-runtime?label=issues&style=flat&labelColor=0b1220&color=a78bfa" />
  <img src="https://img.shields.io/github/last-commit/francescomaiomascio/ice-runtime?label=last%20commit&style=flat&labelColor=0b1220&color=a78bfa" />
  <img src="https://img.shields.io/github/commit-activity/m/francescomaiomascio/ice-runtime?label=commits&style=flat&labelColor=0b1220&color=a78bfa" />
  <img src="https://img.shields.io/github/issues-pr/francescomaiomascio/ice-runtime?label=pull%20requests&style=flat&labelColor=0b1220&color=a78bfa" />
</p>

<!-- MANIFESTO / AXIOMS -->
<p align="center">
  <img
    src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&size=23&weight=500&pause=1400&center=true&vCenter=true&width=780&color=a78bfa&lines=Running+intelligence%2C+beyond+inference.;Authority+precedes+execution.;Inference+is+not+control.;Traceability+is+structural."
  />
</p>

<p align="center">
  <strong>Inference</strong> produces <em>intent</em>.<br/>
  <strong>Runtime responsibility</strong> begins where intent meets reality.
</p>

<p align="center">
  <strong>authorize</strong> · <strong>commit</strong> ·
  <strong>observe</strong> · <strong>govern</strong><br/>
  <em>long-running, stateful systems</em>
</p>

<p align="center">
  Acting is a <strong>structural commitment</strong>,<br/>
  not an implementation detail.
</p>

---

## What I work on

I work on runtime architectures for AI-enabled systems, focusing on what happens  
**after inference**: when proposed actions become **real, persistent state transitions**.

Inference can generate intent, suggestions, or candidate actions.  
**Execution** is the phase where those proposals are evaluated, authorized,  
and applied to system state.  
That transition is neither automatic nor neutral.

In practice, this means deciding:

- **who is allowed to act**
- **when an action is legitimate**
- **what state is allowed to change**
- **how effects are observed, traced, and governed**

In long-running, stateful systems, these decisions *define* behavior.

> [!NOTE]  
> Execution is not plumbing. It is an architectural concern.

---

## Why execution is the hard part

Most AI systems implicitly assume execution is *obvious*, *delegated*,  
or *handled elsewhere*.  
That assumption may hold for prototypes or isolated tasks.  
It breaks down when systems must run continuously, interact with real environments,  
and remain accountable.

The core problem is not intelligence itself.  
It is what happens **after** intelligence produces intent.

> [!WARNING]  
> If inference proposes an action, execution must answer:
> - *Is it allowed?*
> - *Under which authority?*
> - *Which state may change?*
> - *Who is responsible if it fails?*

These are **architectural questions**, not algorithmic ones.

> **Invariant**  
> Inference proposes. Execution decides.

---

## How I build and test these ideas

I build systems end-to-end, from execution semantics down to runtime behavior,  
keeping control flow, state transitions, and side effects **explicit in code**.

I work primarily in **Python**, used as an execution and orchestration language.  
Runtime logic is procedural and organized around a small set of primitives:  
**explicit pipelines**, **state machines**, and **lifecycle phases**.

I deliberately avoid agent frameworks and high-level orchestration toolkits,  
preferring minimal building blocks where execution behavior stays visible.

> [!NOTE]  
> Execution clarity beats abstraction density.

Execution state is handled explicitly through **SQLite / SQL** and **DuckDB**,  
used for checkpoints, transitions, and auditability.  
**SQLAlchemy** is applied only where relational structure is required,  
without turning persistence into an abstraction layer.

Semantic indexing is treated as a bounded capability.  
I use **sentence-transformers** with **FAISS / Chroma**, integrated as inputs to  
execution logic—never as implicit control flow or hidden memory.

Numerical validation relies on **NumPy**, **SciPy**, and **scikit-learn**.  
LLMs are used strictly as **inference components**—primarily open-source models  
via **Hugging Face** and local runtimes—producing proposals that must pass  
explicit authority and state-transition checks.

> [!TIP]  
> Models suggest. Code authorizes. State changes only by rule.

At the systems level, I work directly with **HTTP**, **WebSockets**, **async I/O**,  
filesystem signals, and **CLI/TUI tooling**, keeping operational workflows aligned  
with runtime semantics.

> [!IMPORTANT]  
> ICE is where this approach is exercised today: an execution environment under  
> active construction, used to validate ideas against **real code**, **real state**,  
> and **real failure modes**.

<br/>

<!-- TOOLING / STACK -->
<div align="center" style="max-width: 820px; margin: 48px auto 0 auto;">

<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/vscode/vscode-original.svg" width="44" height="44"/>&nbsp;&nbsp;&nbsp;
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/linux/linux-original.svg" width="44" height="44"/>&nbsp;&nbsp;&nbsp;
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/bash/bash-original.svg" width="44" height="44"/>&nbsp;&nbsp;&nbsp;
<img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original-wordmark.svg" width="44" height="44"/>&nbsp;&nbsp;&nbsp;
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/c/c-original.svg" width="44" height="44"/>&nbsp;&nbsp;&nbsp;
<img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-original.svg" width="44" height="44"/>&nbsp;&nbsp;&nbsp;
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/php/php-original.svg" width="44" height="44"/>

<br/>

<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/html5/html5-original.svg" width="44" height="44"/>&nbsp;&nbsp;&nbsp;
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/nodejs/nodejs-original-wordmark.svg" width="44" height="44"/>&nbsp;&nbsp;&nbsp;
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/fastapi/fastapi-original.svg" width="44" height="44"/>&nbsp;&nbsp;&nbsp;
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/flask/flask-original.svg" width="44" height="44"/>&nbsp;&nbsp;&nbsp;
<img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/mongodb/mongodb-original.svg" width="44" height="44"/>&nbsp;&nbsp;&nbsp;
<img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/mysql/mysql-original-wordmark.svg" width="44" height="44"/>&nbsp;&nbsp;&nbsp;
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/docker/docker-original.svg" width="44" height="44"/>

</div>

<br/>

<!-- STATS + LANGUAGES -->
<p align="center">
  <img
    src="https://github-readme-stats.vercel.app/api?username=francescomaiomascio&show_icons=false&theme=transparent&hide_title=true&hide_border=true&count_private=true&include_all_commits=false&ring_color=a78bfa&text_color=a78bfa"
    width="420"
  />
  <img
    src="https://github-readme-stats.vercel.app/api/top-langs/?username=francescomaiomascio&layout=compact&hide_title=true&theme=transparent&hide_border=true&text_color=a78bfa"
    width="420"
  />
</p>

<!-- SEPARATOR -->
<p align="center">
  <img
    src="https://capsule-render.vercel.app/api?type=rect&height=2&color=0:020617,45:a78bfa,55:a78bfa,100:020617&section=header"
    width="860"
  />
</p>

<!-- ACTIVITY GRAPH -->
<p align="center">
  <img
    src="https://github-readme-activity-graph.vercel.app/graph?username=francescomaiomascio&theme=react-dark&hide_border=true&hide_title=true&bg_color=020617&color=a78bfa&line=a78bfa&point=c4b5fd"
    width="860"
  />
</p>

<p align="center" style="max-width: 680px; margin: 32px auto 18px auto;">
  <span
    style="
      display: inline-block;
      font-size: 0.78em;
      line-height: 1.7;
      letter-spacing: 0.04em;
      opacity: 0.55;
      font-style: italic;
      font-weight: 400;
    ">
    This work is long-term, structural, and research-driven.<br/>
    If it proves valuable, its continuation can be supported.
  </span>
</p>

<p align="center" style="margin-top: 22px; margin-bottom: 8px;">
  <a href="https://www.buymeacoffee.com/francescomaiomascio">
    <img
      src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png"
      height="50"
      alt="Buy me a coffee"
    />
  </a>
</p>
