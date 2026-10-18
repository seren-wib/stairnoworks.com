# stairnoworks.com

[**Status**](#status) | [**What it will do**](#what-it-will-do) | [**How it fits in Stairno**](#how-it-fits-in-stairno) | [**FAQ**](#faq)

**stairnoworks.com** is the site for **Stairno Works**, the **freelance project** of the **Stairno** brand: one place for **taking requests, quoting, deposit payments and tracking progress**, instead of mail threads, messengers and spreadsheets. It is the only Stairno site that takes requests and payments; the hub [stairno.com](https://github.com/seren-wib/stairno.com) only links here. **Nothing is built yet.** This repository holds this README and nothing else.

![GitHub Repo stars](https://img.shields.io/github/stars/seren-wib/stairnoworks.com?style=social)
[![Status](https://img.shields.io/badge/status-planned-lightgrey.svg)](#status)

## Updates

- [2026/10/16] **Repository created.** README only. The site is planned; no code, no domain yet.

## Star History

<a href="https://star-history.com/#seren-wib/stairnoworks.com&Date">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/svg?repos=seren-wib/stairnoworks.com&type=Date&theme=dark" />
    <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/svg?repos=seren-wib/stairnoworks.com&type=Date" />
    <img alt="Star History Chart" src="https://api.star-history.com/svg?repos=seren-wib/stairnoworks.com&type=Date" />
  </picture>
</a>

## Table of Contents

- [Why](#why)
- [Status](#status)
- [What it will do](#what-it-will-do)
- [How it fits in Stairno](#how-it-fits-in-stairno)
- [FAQ](#faq)
- [Contribution](#contribution)

## Why

Taking freelance work alone, the pieces of one job end up in different places:

- The request arrives by mail or messenger, and the details are spread over several replies.
- The quote, the deposit and the deadline live in a spreadsheet the client never sees.
- The client asks "where is it now?" and the answer is another message.

Stairno Works puts them on one site:

- **A request form** tied to a listed service, so every request starts with the same details.
- **Quote, then deposit**, on the same request, so money and scope stay together.
- **A progress timeline** the client can open after signing in, instead of asking.

## Status

Planned. There is no code, no CI, no release and no deployment yet, so there is no quickstart or command list. They will be added here when the first version exists.

- **Domain:** `stairnoworks.com` is not registered yet. It is to be bought through Cloudflare Registrar.
- **Plan:** the first feature plan for this site is in the [atlas-odyssey note of 2026-10-15](https://github.com/seren-wib/atlas-odyssey/blob/develop/docs/notes/2026-10-15.md) (Korean), written before the site got its own repository. Its stack and sign-in choices predate the shared account and design package described below, so treat it as scope, not as a decision.

## What it will do

The planned scope, in priority order:

1. **About and portfolio.** Who takes the work and what was done before.
2. **Service catalog.** Common freelance jobs listed as services, each with a description, a duration and a price or "ask for a quote".
3. **Request intake.** Pick a service, add budget, deadline, description and attachments; a mail notification goes out.
4. **Client sign-in.** A client opens only their own requests.
5. **Quote and deposit payment.** Test or sandbox mode only, until there is a registered business.
6. **Progress tracking.** A timeline from received to quoted, deposit paid, in progress and delivered.
7. **AI help.** Organising a request and answering status questions for the signed-in client, read-only and rate-limited.

Two languages, Korean and English, from the first version. Tax invoices, refunds, real payments and use by other freelancers are out of scope for now.

## How it fits in Stairno

```
Stairno  (brand)
├─ stairno.com           hub: what Stairno is, links to the projects. No sales, no intake.
├─ account.stairno.com   one Stairno account for every site (sign-in through api.stairno.com)
├─ stairno-ui            shared design package @stairno/ui
├─ stairnoworks.com      Works: requests, quotes, deposits, progress   ← this repository
├─ stairnogames.com      Games
└─ stairnolabs.com       Labs
```

- **The hub links here.** [stairno.com](https://github.com/seren-wib/stairno.com) introduces the brand and has a card for Works. It never takes requests or payments; that belongs to this site.
- **Sign-in comes from the shared account.** Stairno sites do not build their own sign-in. Works will be an OpenID Connect client of [account.stairno.com](https://github.com/seren-wib/account.stairno.com), so a client uses the same Stairno account here as on every other Stairno site.
- **The look comes from the shared package.** Every Stairno site looks the same as stairno.com: tokens, header, footer, theme and language toggles come from [`@stairno/ui`](https://github.com/seren-wib/stairno-ui), installed by git tag. This site will not keep its own colours or header.

## FAQ

### 1. Where is the code?

There is none yet. The site is planned; see [Status](#status).

### 2. Does `stairnoworks.com` open anything?

No. The domain is not registered yet.

## Contribution

There is no code to contribute to yet. Issues about the planned scope are welcome. Branch, commit and merge rules will be written in a CONTRIBUTING.md when work starts.

If the idea of one place for freelance requests sounds useful, a ⭐ helps other people find it.
