# Security Policy

## Scope

ArchCanvas is a hosted service at **https://archcanvas.uk**. There is one version — whatever is
live — so there is no supported-versions table: reports are always against production.

This policy covers the hosted application and this repository. The ArchLang compiler is a separate
open-source project with [its own policy](https://github.com/ChanMeng666/archlang/blob/main/SECURITY.md).

## Reporting a vulnerability

**Please do not open a public GitHub issue for a security vulnerability.**

Email **hello@archcanvas.uk** with:

- what the vulnerability is,
- steps to reproduce it, or a proof of concept,
- what an attacker could actually do with it,
- a suggested fix, if you have one.

Please give a reasonable window to fix the issue before disclosing it publicly.

## What we will do

- **Acknowledge** within 48 hours.
- **Assess** — confirm the issue and agree on severity — within 7 days.
- **Fix** confirmed vulnerabilities within 30 days, sooner when severity warrants it.

You will be told when the fix ships.

## Please stay inside these lines

Testing against the live service is fine within the following limits, and this is not an invitation
to anything outside them:

- **Use your own account and your own projects.** Do not access, modify or exfiltrate anyone else's
  projects, plans, share links or billing records.
- **No denial of service**, load testing, or anything that degrades the service for other people.
- **No social engineering**, phishing, or physical attempts against the maintainer or any supplier.
- **Stop at proof.** Once you can demonstrate a vulnerability, stop — do not pivot deeper into the
  system, and do not retain any data you happened to reach.

Reports that follow these rules will not be pursued, and good-faith research is welcome.

## Out of scope

Missing best-practice headers with no demonstrated impact, rate-limit findings without a concrete
exploit, reports produced only by an automated scanner with no verification, self-XSS, and issues in
third-party services we merely consume.

## Credit

With your permission, valid reports are acknowledged publicly once the fix has shipped. There is no
paid bounty programme.
