# Changelog

What has shipped to [archcanvas.uk](https://archcanvas.uk), in plain language. ArchCanvas is a hosted
service that ships continuously, so this is grouped by month rather than by version number — there is
only ever one version, the live one.

Internal refactors, infrastructure and dependency work are not listed here. If a change did not
change what you can see or do, it isn't in this file.

---

## 24 November 2026

- **One free design per person.** Your first account's free design is now given once per person and
  once per browser: a further account for the same email address, or one made in the same browser,
  normally starts without it. Your first account gets its free design at once, on any day.
- **Deleting your account asks for a code.** We email you a 6-digit code; entering it deletes the
  account, its designs and its sign-in in one step.

## 22 November 2026

- **Start your first design without an account.** Type a brief on the home page and the design starts
  at once: you watch it draw and can open its 3D preview. To keep it — and refine, download or share
  it — you create a free account in one step. Keeping a design you started before signing up uses one
  credit, which for a new account is its free one. At times a design cannot be started without an
  account (for example, when one was already started from your network that day); then you sign up
  first. A design you started and did not keep is deleted once it is 7 days old.
- **Renderings removed: the 3D preview is the picture of the building.** Orbit it, step through the
  storeys, look from eye level inside or from the street, and export it as GLB. Renderings made before
  22 November 2026 are no longer shown, and packs no longer include them.
- **Simpler sign-in.** One card: continue with Google, or have a 6-digit code emailed to you — no
  password. Password and GitHub sign-in remain for existing accounts under "Other ways to sign in".
- **Clearer result screen before you keep a design.** The designer's note says what was drawn, what it
  assumed and anything left unresolved, without suggesting edits before you have kept it.

## November 2026

- **A 3D preview of your plan.** A design card and its share page can switch between the plan and a
  3D preview of it, for plans it can show, and the preview works by touch on a phone. The export
  menu can also download the 3D preview as a GLB file.
- **Renderings made from the 3D preview.** Turn the 3D preview to the view you want and make a
  rendering of that view. Every rendering is tagged as an AI-generated impression.
- **Multi-storey plans are designed floor by floor**, so each storey gets its own layout and fit-out.
- **Edits can change a plan's size.** Ask for a smaller or larger plan and the edit resizes it, and
  says so when it could not.
- **A new public site.** The homepage starts with a box to describe your home. A brief typed there
  is kept while you create an account, and your free first design starts straight after sign-up.
- **"Your designs".** The dashboard now shows your designs, with the latest one first.
- **Honest waiting.** The studio says a first design usually takes 2 to 3 minutes, and that you can
  close the page while it carries on.
- **"You decide".** When the designer asks questions before drawing, any of them can be handed back
  to it.
- **A note from the designer.** A first design arrives with a short note on what was drawn and one
  suggested next step.
- **A failed save no longer always costs a credit.** When saving a design fails in a way the system
  can confirm, the credit taken for it is returned automatically.

## October 2026

- **Plans are drawn with real symbols.** Furniture, kitchen and bathroom fixtures, doors and windows
  are now drawn as the things they are — a bed with its pillows, a hob with its rings, a window with
  its glazing — instead of labelled boxes. The ten examples in this repository and on the showcase
  page were redrawn to match.
- **"Your brief" stays with the design.** The checklist that shows which parts of your brief the plan
  meets used to disappear when you dragged a slider or used a quick action. It is now re-checked
  against the changed plan, so it reflects what you are looking at.
- **Better landmarks for screen readers** on the dashboard, account and billing pages: the site
  header is now announced as the page banner, so it can be jumped to and skipped.

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
