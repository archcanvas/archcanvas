# Changelog

What has shipped to [archcanvas.uk](https://archcanvas.uk), in plain language. ArchCanvas is a hosted
service that ships continuously, so this is grouped by month rather than by version number — there is
only ever one version, the live one.

Internal refactors, infrastructure and dependency work are not listed here. If a change did not
change what you can see or do, it isn't in this file.

---

## September 2026

- **A much better designer.** The way a plan is designed was rebuilt around architectural reasoning
  rather than pure geometry: the design is now planned as a whole and reviewed between rounds, which
  shows up as better proportions, better daylight and better circulation. It became the default after
  a blind comparison against the previous approach.
- **Renderings moved to a newer image model** — sharper and more faithful to the drawing they are
  grounded on.
- Various fixes to session expiry and the dashboard, so a stale login no longer leaves parts of the
  page silently empty.

## August 2026

- **Multi-storey plans.** Ask for an upstairs and you get one: one page per storey, an L0/L1 chip row
  on the canvas card, and DXF/PDF export producing one file per level. The checks are building-wide —
  the walk climbs the stairs, and an upstairs bedroom counts toward your brief.
- **One-shot launch.** The dashboard is now the briefing surface. Describe the build, press Enter, and
  you land on the canvas with the design already drawing — one decision, no modal, no second send.
- **A quieter canvas.** Dragging, the minimap, connectors and re-align were removed. They were built
  for a canvas holding several competing designs; the product designs one plan and refines it, so
  they were clutter. The canvas is now a sheet that morphs in place.

## July 2026

- **One strong design, then free edits.** ArchCanvas designs one plan per brief and treats every
  follow-up as feedback on it. Only a fresh generation costs a credit — refining a design in
  conversation is free.
- **Select-to-act.** Click a room, door or window and a floating bar offers actions (Enlarge, Shrink,
  Widen, Move…) scoped to what you clicked. Several of them now run instantly without a model call.
- **Living design.** An edit crossfades the plan in place, with the previous geometry fading out as a
  dashed ghost. A ⇄ chip shows what changed against the parent version, and a timeline scrubber walks
  back through the whole lineage.
- **Review mode.** A ⚑ badge overlays walking routes and pinch points on the drawing, and pins the
  design review's findings where they apply. Each pin offers a free "have AI fix this". It never
  changes anything on its own.
- **Your brief, ticked off.** The checkable parts of your brief — room counts, areas, adjacencies,
  windows — are validated against the finished plan and shown as a ✓/✗ list, re-checked after every
  edit against the *original* brief.
- **Grounded renderings.** Renderings are now produced from a raster of the actual compiled plan, so
  what you see matches the geometry instead of being imagined separately.
- **Parametric tweaks.** Drag sliders for a plan's parameters — room sizes, counts, wall thickness —
  and it recompiles live. Saving forks a new version. No model call, no credit.
- **Typology presets** — constrain a design to a building program (residential, accessible clinic,
  open-plan office, passive house).
- **Clarifying questions.** A thin brief now gets 2–5 questions as an inline form before anything is
  designed, instead of a guess.
- **Design critique** — a written review of circulation, daylight, program and proportion that cites
  the plan's own measured walk distances and door widths.
- **Voice input** for the brief.
- **New identity**, and the public pages were rebuilt around it.
- **The site moved to [archcanvas.uk](https://archcanvas.uk).** The old address redirects.

## Before July 2026

The first public version: describe a brief, get floor plans and renderings on an infinite canvas,
buy credits in one-time packs. Plans were originally drawn freehand by a model; they are now written
as [ArchLang](https://github.com/ChanMeng666/archlang) source and compiled, which is what made
dimensions, exports and checking possible at all.
