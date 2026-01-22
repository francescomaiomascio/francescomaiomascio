<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&height=96&section=header&text=Authority%20precedes%20execution.&font=IBM+Plex+Sans&fontSize=19&fontAlignY=35&color=0:020617,40:6d28d9,60:a78bfa,100:020617&fontColor=d1d5db" width="100%" />
</p>

## How I work

I don’t approach system design from first principles in isolation.  
My work is shaped by friction with **real systems in production** —
systems that run continuously, evolve over time,
and fail in ways theory rarely anticipates.

What I’ve learned is that most architectural problems today
do not stem from missing capabilities,
but from **unclear responsibility**:
implicit decisions,
invisible transitions,
and no reliable way to explain *why* something happened after the fact.

My approach starts by making those boundaries explicit.

I design systems **from the outside in**:
starting from observable behavior,
then working backward to define
which transitions are allowed,
which are forbidden,
and which must remain undecided.

I favor execution paths that are **boring, inspectable, and reconstructible**.  
If a system acts, I want to be able to point to the exact sequence
that led there — without relying on emergent behavior
or opaque orchestration.

Python is the medium I use to express this discipline:
not as an abstraction engine,
but as a way to model control flow,
lifecycle phases,
and state transitions explicitly.

I avoid agent frameworks and implicit schedulers,
because they trade short-term convenience
for long-term opacity.

> [!TIP]  
> *Models suggest. Code authorizes. State changes only by rule.*

Persistence is treated as part of system semantics, not infrastructure.  
I use **SQLite / SQL** and **DuckDB** to anchor execution in durable state,
support recovery,
and make post-hoc reasoning possible.

**SQLAlchemy** is used sparingly and locally —
never in ways that hide ownership of state
or blur transition boundaries.

Semantic indexing and vector search  
(*sentence-transformers + FAISS / Chroma*)  
are inputs to reasoning, not drivers of behavior.  
They can inform decisions,
but they never *make* them.

LLMs are constrained strictly to inference.  
They produce proposals —
never actions.

Everything beyond that boundary is handled
by explicit rules and declared transitions.

> [!IMPORTANT]  
> **ICE** is where this approach is exercised today —
> against *real code paths*, *real state*,
> and *real failure modes*.
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

</div>

</br>

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

<p align="center"><a href="https://www.buymeacoffee.com/francescomaiomascio"><img src="https://img.buymeacoffee.com/button-api/?text=&emoji=&slug=francescomaiomascio&button_colour=BD5FFF&font_colour=ffffff&font_family=Cookie&outline_colour=000000&coffee_colour=FFDD00" height="64" /></a></p>

<!-- BOTTOM WAVING FOOTER -->
<p align="center" style="margin-top: 18px;">
  <img
    src="https://capsule-render.vercel.app/api?type=waving&height=76&section=footer&color=0:020617,40:6d28d9,60:a78bfa,100:020617"
    width="100%"
  />
</p>
