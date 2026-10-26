# Beamable (beamable)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Beamable is a cloud backend platform purpose-built for games and interactive applications, providing REST APIs and SDK integrations for Unity, Unreal, and web environments. The platform delivers production-ready services covering player identity and authentication, virtual currency and economy, inventory management, leaderboards, matchmaking, live events, and analytics. Developers can extend the platform with custom C# microservices and scheduled jobs, deploying server-side logic without managing infrastructure. Beamable is backed by AWS and has served over 30 million players, offering a LiveOps portal, CLI tooling, and content management for games-as-a-service operations.

- **APIs.json:** https://raw.githubusercontent.com/api-evangelist/beamable/refs/heads/main/apis.yml
- **Naftiko:** https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=beamable-api-evangelist&utm_content=repo

## Tags

- Game Backend
- LiveOps
- Player Accounts
- Virtual Currency
- Inventory
- Leaderboards
- Matchmaking
- Microservices
- Unity
- Unreal
- Game Economy
- Analytics

## APIs

| API | Description |
|-----|-------------|
| Player Accounts API | Player identity, authentication, and account management with OAuth integrations |
| Game Economy API | Virtual currency, inventory, and in-game store management |
| Leaderboards API | Competitive leaderboards with global, friend-based, and partitioned rankings |
| Live Events API | Scheduling and management for live events, announcements, and player mail |
| Microservices API | Custom C# server-side logic deployed as managed microservices |

## Plans, Rate Limits, and FinOps

| Resource | Location |
|----------|----------|
| Plans and Pricing | [plans/beamable-plans-pricing.yml](plans/beamable-plans-pricing.yml) |
| Rate Limits | [rate-limits/beamable-rate-limits.yml](rate-limits/beamable-rate-limits.yml) |
| FinOps Framework | [finops/beamable-finops.yml](finops/beamable-finops.yml) |

Beamable uses a subscription-plus-consumption billing model. Pricing tiers are:

| Plan | Price/Month | API Calls Included | MAU | Microservices |
|------|-------------|-------------------|-----|---------------|
| Free Trial | $0 (90 days) | — | — | — |
| Developer | $125 | 12.5M | 1,000 | 3 |
| Studio | $595 | 59.5M | 30,000 | 10 |
| Pro | $1,895 | 189.5M | 100,000 | 25 |
| Enterprise | $3,500+ | 350M+ | Unlimited | 75+ |

Overage: $100 per 10M additional API calls (standard); $10 per 1M at Enterprise scale. Each API call is subject to a 10KB bandwidth limit. Additional microservices: $20/month each. No separate storage or bandwidth charges.

## Timestamps

- **Created:** 2026-06-12
- **Modified:** 2026-06-12

## Common Resources

| Type | URL |
|------|-----|
| Website | https://beamable.com/ |
| Documentation | https://docs.beamable.com/docs/beamable-overview |
| GitHub Org | https://github.com/beamable |
| LinkedIn | https://www.linkedin.com/company/beamable |
| Blog | https://beamable.com/category/blog |
| Pricing | https://beamable.com/pricing |
| Status Page | https://beamable.github.io/status/ |
| X / Twitter | https://twitter.com/Beamable |

## Maintainers

| Name | Email |
|------|-------|
| Kin Lane | kin@apievangelist.com |
