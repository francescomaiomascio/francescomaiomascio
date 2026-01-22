<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&height=96&section=header&text=Authority%20precedes%20execution.&font=IBM+Plex+Sans&fontSize=19&fontAlignY=35&color=0:020617,40:6d28d9,60:a78bfa,100:020617&fontColor=d1d5db" width="100%" />
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

## Execution model

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


<!-- TOOLING / STACK -->
<div align="center">

<img src="https://techstack-generator.vercel.app/python-icon.svg" width="48"/>
<img src="https://techstack-generator.vercel.app/js-icon.svg" width="48"/>
<img src="https://techstack-generator.vercel.app/mysql-icon.svg" width="48"/>
<img src="https://techstack-generator.vercel.app/ts-icon.svg" width="48"/>
<img src="https://techstack-generator.vercel.app/aws-icon.svg" width="48"/>
<img src="https://techstack-generator.vercel.app/csharp-icon.svg" width="48"/>

<img src="https://techstack-generator.vercel.app/django-icon.svg" width="48"/>
<img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/git/git-original.svg" width="48"/>
<img src="https://skillicons.dev/icons?i=docker" width="48"/>

<img src="https://skillicons.dev/icons?i=mongodb" width="48"/>
<img src="https://skillicons.dev/icons?i=linux" width="48" height="48"/>

</br>

</div>
<!-- ACTIVITY GRAPH -->
<p align="center">
  <img
    src="https://github-readme-activity-graph.vercel.app/graph?username=francescomaiomascio&theme=minimal&hide_border=true&hide_title=true&bg_color=00000000&color=8b5cf6&line=8b5cf6&point=ddd6fe"
    width="660"
  />
</p>

<p align="center" style="max-width: 560px; margin: 28px auto 16px auto;">
  <span style="opacity: 0.55; font-size: 0.82em;">
    This work is long-term, structural, and research-driven.<br/>
    <em>Support sustains continuity, not direction.</em>
  </span>
</p>

<p align="center" style="margin-top: 10px;">
  <a href="https://www.buymeacoffee.com/francescomaiomascio">
    <img
      src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png"
      height="36"
      alt="Support this work"
      style="opacity: 0.8;"
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
