<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&height=120&section=header&text=Authority%20precedes%20execution.&fontSize=26&fontAlignY=42&color=0:020617,40:6d28d9,60:a78bfa,100:020617&fontColor=c4b5fd" width="100%" />
</p>

## What I work on

I design **runtime architectures for AI-enabled systems**, focused on what happens  
*after inference* — when proposed actions become **real, persistent state transitions**.

> [!NOTE]  
> *Execution is an architectural concern, not plumbing.*

Inference proposes intent; **execution decides** whether that intent is legitimate, authorized, and observable.  
Execution defines **who can act**, **when**, **what state may change**, and **how responsibility is tracked**.  
In *long-running systems*, this is not an implementation detail — it **is** the system’s behavior.

Most AI systems treat execution as obvious or external.  
That assumption fails once systems run continuously, affect real state, and must remain accountable.  
The problem is not intelligence, but what happens *after* intelligence produces intent.

> [!IMPORTANT]  
> **Invariant** — *Inference proposes. Execution decides.*

```python
def __post_init__(self) -> None:
    self._normalize_time()
    self._seal_integrity()
    self._enforce_invariants()
```

## How I build systems

I build systems **end-to-end**, keeping *control flow*, *state transitions*, and *side effects* explicit.
Execution behavior is never implicit, inferred, or delegated to opaque layers.

Python is used as an **execution and orchestration language**, structured around
*explicit pipelines*, *state machines*, and *lifecycle phases*.
I deliberately avoid agent frameworks and black-box orchestration;
minimal primitives keep execution behavior *observable*.

> [!TIP]  
> *Models suggest. Code authorizes. State changes only by rule.*

State is handled explicitly via **SQLite / SQL** and **DuckDB** for checkpoints,
reproducibility, and auditability.
**SQLAlchemy** is used selectively — *never* as an abstraction boundary.

Semantic indexing is treated as a **bounded input capability**
(*sentence-transformers + FAISS / Chroma*), never as implicit control flow.

LLMs are used strictly for **inference**:
they produce proposals that must pass *explicit authority* and *state-transition checks*.

At the systems level, I work directly with **HTTP**, **WebSockets**, **async I/O**,
filesystem signals, and **CLI / TUI tooling**.

> [!IMPORTANT]  
> **ICE** is where this approach is exercised today — against *real code*, *real state*, and *real failure modes*.

<br/>

<!-- TOOLING / STACK -->
<div align="center">

<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/linux/linux-original.svg" width="30" height="30"/>
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/bash/bash-original.svg" width="30" height="30"/>
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg" width="30" height="30"/>
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/c/c-original.svg" width="30" height="30"/>
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/docker/docker-original.svg" width="30" height="30"/>
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/kubernetes/kubernetes-plain.svg" width="30" height="30"/>
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/git/git-original.svg" width="30" height="30"/>
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/vscode/vscode-original.svg" width="30" height="30"/>
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-original.svg" width="30" height="30"/>
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/nodejs/nodejs-original.svg" width="30" height="30"/>
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/flask/flask-original.svg" width="30" height="30"/>
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/mongodb/mongodb-original.svg" width="30" height="30"/>
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/mysql/mysql-original.svg" width="30" height="30"/>

</div>

<br/>

<!-- ACTIVITY GRAPH -->
<p align="center">
  <img
    src="https://github-readme-activity-graph.vercel.app/graph?username=francescomaiomascio&theme=minimal&hide_border=true&hide_title=true&bg_color=00000000&color=8b5cf6&line=8b5cf6&point=ddd6fe"
    width="660"
  />
</p>

<p align="center" style="max-width: 620px; margin: 26px auto 14px auto;">
  <span>
    This work is long-term, structural, and research-driven.<br/>
    <em>Support sustains continuity — it does not shape direction.</em>
  </span>
</p>

<p align="center" style="margin-top: 12px; margin-bottom: 4px;">
  <a href="https://www.buymeacoffee.com/francescomaiomascio">
    <img
      src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png"
      height="40"
      alt="Support this work"
      style="opacity: 0.85;"
    />
  </a>
</p>

<!-- BOTTOM WAVING FOOTER -->
<p align="center" style="margin-top: 18px;">
  <img
    src="https://capsule-render.vercel.app/api?type=waving&height=76&section=footer&color=0:020617,40:6d28d9,60:a78bfa,100:020617"
    width="100%"
  />
</p>
