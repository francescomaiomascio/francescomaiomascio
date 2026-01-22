<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&height=96&section=header&text=Authority%20precedes%20execution.&font=IBM+Plex+Sans&fontSize=19&fontAlignY=35&color=0:020617,40:6d28d9,60:a78bfa,100:020617&fontColor=d1d5db" width="100%" />
</p>

## How I work

Most architectural failures today are not caused by missing features,
but by **unclear responsibility**:
implicit decisions, opaque transitions,
and no reliable way to explain *why* something happened.

I work by making those boundaries explicit.

Systems are defined **from observable behavior backward**:
what happens is visible first;
what is *allowed* to happen is constrained next.
Everything else is implementation detail.

I favor execution paths that are **boring, inspectable, and reconstructible**.
If a system acts, I expect to trace that action
through declared authority and durable state —
without inference or guesswork.

Python is the medium I use to express this discipline:
explicit control flow, lifecycle phases,
and state transitions.
I avoid agent frameworks and implicit schedulers;
they trade convenience for opacity.

> [!TIP]  
> *Models suggest. Code authorizes. State changes only by rule.*

Persistence is treated as part of system semantics.
**SQLite / SQL** and **DuckDB** anchor execution in durable state
and make post-hoc reasoning possible.

Semantic indexing (*sentence-transformers + FAISS / Chroma*)
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
<img src="https://skillicons.dev/icons?i=docker" width="48"/>
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
<p align="center" style="margin: 8px 0;">
  <a href="https://www.buymeacoffee.com/francescomaiomascio">
    <img
      src="https://img.buymeacoffee.com/button-api/?text=&emoji=&slug=francescomaiomascio&button_colour=BD5FFF&font_colour=ffffff&font_family=Cookie&outline_colour=000000&coffee_colour=FFDD00"
      height="64"
    />
  </a>
</p>

<p align="center" style="margin: 8px 0;">
  <a href="https://www.paypal.com/donate/?hosted_button_id=JWGLSTD4U9NEE">
    <img
      src="assets/pp-butt.png"
      width="240"
      alt="Donate with PayPal"
    />
  </a>
</p>
