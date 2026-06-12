# Beamable (beamable)

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
