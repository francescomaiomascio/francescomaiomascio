<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&height=96&section=header&text=Authority%20precedes%20execution.&font=IBM+Plex+Sans&fontSize=19&fontAlignY=35&color=0:020617,40:6d28d9,60:a78bfa,100:020617&fontColor=d1d5db" width="100%" />
</p>

## How I work

I work on systems that already exist.
Systems that run continuously, evolve under load,
and fail in ways no design document anticipates.

Most architectural failures today are not caused by missing features,
but by **unclear responsibility**:
implicit decisions,
opaque transitions,
and no reliable way to explain *why* something happened.

My approach starts by making those boundaries explicit.

I design systems **from observable behavior backward**.
What the system does comes first;
what it is *allowed* to do is defined next.
Everything else is implementation detail.

I favor execution paths that are **boring, inspectable, and reconstructible**.
If a system acts, I expect to trace that action
through explicit steps, declared authority,
and durable state — without inference or guesswork.

Python is the medium I use to express this discipline:
to model control flow, lifecycle phases,
and state transitions explicitly.
I avoid agent frameworks and implicit schedulers,
because they trade convenience for opacity.

> [!TIP]  
> *Models suggest. Code authorizes. State changes only by rule.*

Persistence is treated as part of system semantics.
**SQLite / SQL** and **DuckDB** anchor execution in durable state,
enable recovery,
and make post-hoc reasoning possible.

Semantic indexing and vector search
(*sentence-transformers + FAISS / Chroma*)
may inform decisions,
but never drive control flow.

LLMs are constrained strictly to inference.
They produce proposals — never actions.

> [!IMPORTANT]  
> **ICE** is where this approach is exercised —
> against *real code*, *real state*,
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
