<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="./assets/brand/wordmark-ondark.svg" />
  <img src="./assets/brand/wordmark-onlight.svg" alt="ArchCanvas" width="460" />
</picture>

### Describe your build. Get a floor plan you can act on.

Describe your home in plain English. Get a dimensioned floor plan back, with a written list of everything it could not get right.

<a href="https://archcanvas.uk"><img src="./.github/readme/pill-open-the-studio.svg" height="40" alt="Open the studio"></a> <a href="examples/"><img src="./.github/readme/pill-examples.svg" height="40" alt="Examples"></a> <a href="ROADMAP.md"><img src="./.github/readme/pill-roadmap.svg" height="40" alt="Roadmap"></a> <a href="https://github.com/ChanMeng666/archlang"><img src="./.github/readme/pill-archlang.svg" height="40" alt="ArchLang"></a>

</div>

<br>

<a href="https://archcanvas.uk/"><img src="./.github/readme/card.svg" width="100%" alt="ArchCanvas, an AI architectural designer: describe your home and get a dimensioned floor plan. The studio takes a brief, drafts the plan in passes, moves a wall from an edit in plain words, lists what it could not get right, then renders and exports it."></a>

<br>

<video src="https://github.com/user-attachments/assets/8986f197-f06c-49a7-ac4f-ddcab7f51abd" controls width="100%"></video>

<br>

## Try it

Open the studio at **[archcanvas.uk](https://archcanvas.uk)** and type a brief. A sentence is enough to start:

> *Three bedrooms, open kitchen-living, north-facing, roughly 110 m².*

You get one floor plan on an infinite canvas. Then you change it by talking to it: move a wall, resize a room, add an upstairs.

## Why it is different

- **One plan, not fifty.** A single consistent plan you shape until it is right.
- **Checked before you see it.** A compiler walks every route, measures every door and confirms every room is reachable. What it could not resolve is written on the drawing.
- **Yours to take away.** Export SVG, PNG, DXF, PDF or the editable source, one file per storey.

```mermaid
flowchart LR
    B([Brief]) --> S[Plan written<br/>as source]
    S --> C[Compiler<br/>checks it]
    C --> P[Plan on<br/>the canvas]
    P -->|edit in plain words| S
    P --> O([SVG · PNG · DXF · PDF])
```

It is a concept plan, not a stamped permit set or construction documents.

## For your agent

This page is all a person needs. For the rest, clone the repo and point your coding agent at [`docs/overview.md`](docs/overview.md). The ten plans in [`examples/`](examples/) ship with their source, and each one recompiles on your own machine:

```bash
npx @chanmeng666/archlang compile examples/garden-office/plan.arch -o plan.svg
```

<sub>[Full overview](docs/overview.md) · [FAQ](docs/faq.md) · [Changelog](CHANGELOG.md) · [Discussions](https://github.com/archcanvas/archcanvas/discussions) · [Issues](https://github.com/archcanvas/archcanvas/issues) · [Contributing](CONTRIBUTING.md) · [Support](SUPPORT.md) · [Security](SECURITY.md) · [Two-minute film](https://youtu.be/rUZAiXgt9JY) · [License](LICENSE)</sub>

<sub>ArchCanvas is a commercial product and its application source is not open. The engine underneath, [ArchLang](https://github.com/ChanMeng666/archlang), is open source (MIT). Built by [Chan Meng](https://github.com/ChanMeng666).</sub>
