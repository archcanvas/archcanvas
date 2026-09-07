# Contributing

Thanks for being here. A quick note on what this repository is, so nobody spends an evening on
something that can't be merged.

## What this repository is

**ArchCanvas is a commercial product and its application source is not public.** This repository is
the product's public home: the examples, the documentation, the roadmap, the issue tracker and the
community. There is no application code here to send a pull request against.

That is not a slight on contribution — it is just honest about where the seams are. The parts of the
system that *are* open live in a different repository:
**[ArchLang](https://github.com/ChanMeng666/archlang)**, the MIT-licensed DSL and compiler that draws
every plan ArchCanvas produces. If you want to change how a wall, a door swing or a dimension string
is *drawn*, that is where the code is, and pull requests there are genuinely welcome.

## What helps most here

**1. Tell us about a plan that came out wrong.** This is the single most valuable thing you can
contribute. Open a [Plan quality report](https://github.com/archcanvas/archcanvas/issues/new/choose)
with the brief you gave and the drawing you got back, and say what a person who knows buildings would
have done differently. Design quality is the hard part of this product, and a specific bad plan is
worth more than a hundred general opinions.

**2. Report a bug.** Something broke, hung, charged you wrongly, or exported a file that won't open.
Use the [Bug report](https://github.com/archcanvas/archcanvas/issues/new/choose) template.

**3. Ask for something.** Feature requests go through the
[Feature request](https://github.com/archcanvas/archcanvas/issues/new/choose) template. Half of the
[roadmap](ROADMAP.md) started as one.

**4. Show what you made.** Post it in
[Discussions → Show & tell](https://github.com/archcanvas/archcanvas/discussions). Plans people
actually made are the best documentation this project has.

**5. Fix the docs.** Pull requests are accepted for the Markdown in this repository — a wrong link, a
confusing FAQ answer, a typo. Keep them small and self-explanatory.

**6. Add an example.** If you have designed something with ArchCanvas that would teach other people
something, a PR adding `examples/<slug>/plan.arch` plus its compiled `plan.svg` is welcome. Please
confirm in the PR that you are happy for it to be published under this repository's CC BY 4.0 terms
(see [LICENSE](LICENSE)), and that the plan is not of a real private residence you don't own.

## What will be closed

- Pull requests adding application code, since there is no application here.
- Requests to open-source ArchCanvas. The answer is no, and the reasoning is in the
  [README](README.md#built-on-archlang): the substrate is open, the product is not.
- Security vulnerabilities filed as public issues — please follow [SECURITY.md](SECURITY.md) instead.

## Ground rules

Be decent to each other; the [Code of Conduct](CODE_OF_CONDUCT.md) applies everywhere in this
repository. Account, billing and refund questions are handled privately — see
[SUPPORT.md](SUPPORT.md) rather than opening an issue with your order details in it.

This is a solo-maintained project. Responses are usually quick and occasionally not; patience is
appreciated.
