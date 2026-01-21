<!-- TOP WAVING HEADER -->
<p align="center">
  <img
    src="https://capsule-render.vercel.app/api?type=waving&height=110&section=header&color=0:020617,40:6d28d9,60:a78bfa,100:020617"
    width="100%"
  />
</p>

<!-- MANIFESTO / AXIOMS -->
<p align="center">
  <img
    src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&size=23&weight=500&pause=1400&center=true&vCenter=true&width=780&color=a78bfa&lines=Running+intelligence%2C+beyond+inference.;Authority+precedes+execution.;Inference+is+not+control.;Traceability+is+structural."
  />
</p>


<!-- GITHUB STATUS / SIGNALS -->
<p align="center">
  <img src="https://img.shields.io/github/stars/francescomaiomascio/ice-runtime?label=stars&style=flat&labelColor=0b1220&color=a78bfa" />
  <img src="https://img.shields.io/github/issues/francescomaiomascio/ice-runtime?label=issues&style=flat&labelColor=0b1220&color=a78bfa" />
  <img src="https://img.shields.io/github/last-commit/francescomaiomascio/ice-runtime?label=last%20commit&style=flat&labelColor=0b1220&color=a78bfa" />
  <img src="https://img.shields.io/github/commit-activity/m/francescomaiomascio/ice-runtime?label=commits&style=flat&labelColor=0b1220&color=a78bfa" />
  <img src="https://img.shields.io/github/issues-pr/francescomaiomascio/ice-runtime?label=pull%20requests&style=flat&labelColor=0b1220&color=a78bfa" />
</p>

<p align="center">
  <strong>Inference</strong> produces <em>intent</em> · execution governs reality<br/>
  <strong>authorize</strong> · <strong>commit</strong> · <strong>observe</strong> · <strong>govern</strong> —
  <em>long-running, stateful systems</em>
</p>

</br>

```python
def __post_init__(self) -> None:
    self._normalize_time()
    self._seal_integrity()
    self._enforce_invariants()

```
## What I work on

I design **runtime architectures for AI-enabled systems**, focused on what happens  
**after inference**—when proposed actions become **real, persistent state transitions**.

Inference proposes intent; **execution decides** whether that intent is legitimate, authorized, and observable.  
Execution defines **who can act**, **when**, **what state may change**, and **how responsibility is tracked**.  
In long-running systems, this is not an implementation detail — it *is* the system’s behavior.

Most AI systems treat execution as obvious or external.  
That assumption fails once systems run continuously, affect real state, and must remain accountable.  
The problem is not intelligence, but what happens **after** intelligence produces intent.

> [!NOTE]  
> Execution is an architectural concern, not plumbing.

> [!IMPORTANT]  
> **Invariant** — Inference proposes. Execution decides.

## How I build systems

I build systems end-to-end, keeping **control flow, state transitions, and side effects explicit**.

Python is used as an **execution and orchestration language**, structured around  
**explicit pipelines**, **state machines**, and **lifecycle phases**.  
I avoid agent frameworks and opaque orchestration layers; minimal primitives keep execution behavior visible.

State is handled explicitly via **SQLite / SQL** and **DuckDB** for checkpoints and auditability.  
**SQLAlchemy** is used selectively, never as an abstraction boundary.

Semantic indexing is a bounded input capability  
(**sentence-transformers + FAISS / Chroma**), never implicit control flow.

LLMs are used strictly for **inference**—producing proposals that must pass  
explicit authority and state-transition checks.

> [!TIP]  
> Models suggest. Code authorizes. State changes only by rule.

At the systems level I work directly with **HTTP**, **WebSockets**, **async I/O**,  
filesystem signals, and **CLI/TUI tooling**.

> [!IMPORTANT]  
> **ICE** is where this approach is exercised today—against **real code**,  
> **real state**, and **real failure modes**.


<br/>

<!-- TOOLING / STACK -->
<div align="center" style="max-width: 820px; margin: 40px auto 0 auto;">

<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/vscode/vscode-original.svg" width="40" height="40"/>&nbsp;&nbsp;
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/linux/linux-original.svg" width="40" height="40"/>&nbsp;&nbsp;
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/bash/bash-original.svg" width="40" height="40"/>&nbsp;&nbsp;
<img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original-wordmark.svg" width="40" height="40"/>&nbsp;&nbsp;
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/c/c-original.svg" width="40" height="40"/>&nbsp;&nbsp;
<img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-original.svg" width="40" height="40"/>&nbsp;&nbsp;
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/php/php-original.svg" width="40" height="40"/>

<br/>

<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/html5/html5-original.svg" width="40" height="40"/>&nbsp;&nbsp;
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/nodejs/nodejs-original-wordmark.svg" width="40" height="40"/>&nbsp;&nbsp;
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/fastapi/fastapi-original.svg" width="40" height="40"/>&nbsp;&nbsp;
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/flask/flask-original.svg" width="40" height="40"/>&nbsp;&nbsp;
<img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/mongodb/mongodb-original.svg" width="40" height="40"/>&nbsp;&nbsp;
<img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/mysql/mysql-original-wordmark.svg" width="40" height="40"/>&nbsp;&nbsp;
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/docker/docker-original.svg" width="40" height="40"/>

</div>

<br/>



<!-- ACTIVITY GRAPH -->
<p align="center">
  <img
    src="https://github-readme-activity-graph.vercel.app/graph?username=francescomaiomascio&theme=react-dark&hide_border=true&hide_title=true&bg_color=020617&color=a78bfa&line=a78bfa&point=c4b5fd"
    width="700"
  />
</p>

<p align="center" style="max-width: 680px; margin: 28px auto 16px auto;">
  <span
    style="font-size:0.78em; line-height:1.6; letter-spacing:0.04em; opacity:0.55; font-style:italic;">
    This work is long-term, structural, and research-driven.</br>  
    If it proves valuable, its continuation can be supported.
  </span>
</p>

<p align="center" style="margin-top: 20px;">
  <a href="https://www.buymeacoffee.com/francescomaiomascio">
    <img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" height="48" />
  </a>
</p>

<!-- BOTTOM WAVING FOOTER -->
<p align="center">
  <img
    src="https://capsule-render.vercel.app/api?type=waving&height=90&section=footer&color=0:020617,40:6d28d9,60:a78bfa,100:020617"
    width="100%"
  />
</p>
