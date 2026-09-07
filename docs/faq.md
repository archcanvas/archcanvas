# FAQ

The questions that come up most. If yours isn't here, ask in
[Discussions](https://github.com/archcanvas/archcanvas/discussions).

---

## About the plans

### Can I get a building permit with this?

No, and you should be suspicious of any AI tool that says otherwise.

ArchCanvas gives you a **concept plan you can think and decide with, and hand to a professional** —
dimensioned, internally consistent, and exportable as DXF/PDF. It is **not** a stamped permit set or
construction documents, and we don't pretend it is. What it does is get you a solid, buildable-shaped
starting point in minutes for a few dollars, so that when you *do* pay a draftsperson or architect for
permit-ready drawings, you're not paying them to figure out what you want from scratch — you're paying
them to finish something real.

### Does it check structure, services or building codes?

No. It checks *geometry and use*: that walls close, that rooms are reachable, that doors are wide
enough to pass through, that dimensions are consistent, and that the plan matches the brief you gave
it. Structure, services, fire and code compliance are a qualified professional's job, and nothing
here substitutes for one.

### Why one plan instead of several options?

ArchCanvas designs one strong floor plan for you — properly dimensioned, walls that actually close —
then refines it with you until it's right. The bet is deliberate: one consistent plan you shape for
free beats several rough options you have to choose between blind. If that bet is wrong for you, the
free tier costs nothing to check.

You can still ask for variations explicitly, and you'll get them.

### Why does it take so long?

A generation takes about 100–160 seconds because we compile and check the geometry before showing it
to you. That's a deliberate bet: one strong, consistent plan you then refine for free, instead of
several rough options in a minute that you have to choose between blind. If that trade is wrong for
you, the free tier costs nothing to find out.

### Something in the plan is wrong. What do I do?

Two things, and please do both:

1. **Tell it.** Say what's wrong in the conversation — "the bathroom has no window", "move the stairs
   to the hallway". Edits are free and land on the canvas in place.
2. **Tell us.** Open a
   [plan quality report](https://github.com/archcanvas/archcanvas/issues/new/choose) with the brief
   and the drawing. That is the most useful thing anyone sends us.

### What does it do when it can't satisfy my brief?

It writes it on the drawing. If a room wouldn't fit, or an adjacency you asked for couldn't be
honoured, that shows up as a named item rather than being quietly dropped and left for you to find.

---

## Files and exports

### What can I export?

SVG and PNG from the browser; **DXF** and **PDF** from the server; and the editable **ArchLang
source** itself. Multi-storey plans export one file per storey.

### What is ArchLang, and why do I care?

[ArchLang](https://github.com/ChanMeng666/archlang) is the open-source (MIT) language and compiler
that draws every ArchCanvas plan. The AI writes `.arch` source; the compiler turns it into the
drawing. You care for two practical reasons: the geometry is consistent because a compiler produced
it rather than a picture generator, and you can take the source with you — it isn't a format only we
can read. Every example in [`examples/`](../examples/) is a real one, and you can recompile it
yourself:

```bash
npx @chanmeng666/archlang compile examples/garden-office/plan.arch -o plan.svg
```

### Can I use the plans commercially?

Yes. Plans you generate are yours to use, including for a real build — subject to the obvious caveat
above that they are concept drawings and a professional still has to take them the rest of the way.
The [terms](https://archcanvas.uk/terms) are the authority here.

### Will my DXF open in real CAD software?

Yes — that's the point of exporting DXF rather than an image. If one doesn't open in your tool,
that's a bug worth [reporting](https://github.com/archcanvas/archcanvas/issues/new/choose).

---

## Credits and billing

### How does pricing work?

No subscription. You design a house a handful of times in your life, not every month — so you pay per
result you keep, with credits that never expire. You're never billed for a month you didn't use.

One credit buys one generation: the plan, its rendering and its review. **Refining that design in
conversation is free**, and once you've bought any pack, refinement and renderings are unlimited.

The free tier is one complete floor plan plus 10 rounds of refinement and 2 renderings, without a
card.

### Do credits expire?

No.

### Can I get a refund?

Email **hello@archcanvas.uk** — please don't put order details in a public issue. Refunds are
handled case by case and reasonably.

---

## Account and data

### What happens to my brief and my plans?

The short answer: your brief is sent to an AI provider to design the plan, and your projects are
stored so you can come back to them. The full and authoritative answer — who processes what, where,
and for how long — is the [privacy policy](https://archcanvas.uk/privacy).

### Are my projects public?

No. A project is private to your account unless you create a share link for it, which is a read-only
URL you can give to anyone. Deleting the share link revokes it.

### Can I delete my account?

Yes — see the [privacy policy](https://archcanvas.uk/privacy) for how, and what is deleted.

---

## The project itself

### Is ArchCanvas open source?

No. ArchCanvas is a commercial, closed-source product; this repository is its public home — examples,
docs, roadmap, issues and community. The engine underneath, ArchLang, **is** open source under MIT
and is developed [in the open](https://github.com/ChanMeng666/archlang).

### Who builds this?

One person — [Chan Meng](https://github.com/ChanMeng666) — in public. That's also why support is
best-effort and the roadmap is a guess rather than a plan.

### How do I follow along?

Watch this repository, or read the [changelog](../CHANGELOG.md).
