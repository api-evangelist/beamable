# Beamable GraphQL Schema

## Overview

This conceptual GraphQL schema models the Beamable game backend platform for LiveOps. Beamable provides production-ready services for player identity, virtual economy, inventory management, leaderboards, tournaments, live events, cloud save, groups, and in-game messaging. The schema is derived from the Beamable REST API surface documented at https://docs.beamable.com/reference/api-reference and the Beamable platform overview at https://docs.beamable.com/docs/beamable-overview.

The schema file is located at: `graphql/beamable-schema.graphql`

## Domain Coverage

### Player Identity and Session Management

Types `Player`, `PlayerDetails`, `PlayerStatus`, `Session`, `SessionDetails`, `Token`, `Auth`, and `OAuthDetails` cover the full player lifecycle from guest login through third-party OAuth (Facebook, Google, Apple, Steam) and multi-device session handling.

### Virtual Economy

Types `Currency`, `CurrencyDetails`, `CurrencyAmount`, `VirtualCurrency`, and `CurrencyContent` model soft, hard, and premium currencies. The `PlayerInventory` type aggregates currency balances and item holdings per player.

### Inventory and Content

Types `Item`, `ItemDetails`, `ItemContent`, `ContentItem`, `ContentDetails`, and `ContentType` represent Beamable's content management system, where game designers publish item and currency definitions that the runtime resolves into player inventory entries.

### Leaderboards

Types `LeaderBoard`, `LeaderBoardDetails`, `Ranking`, `Score`, and `Entry` support global, partitioned, and friend-based competitive rankings with configurable reset schedules.

### Tournaments

Types `Tournament`, `TournamentDetails`, `TournamentStage`, `TournamentEntry`, `TournamentChampion`, and `TournamentReward` model multi-stage competitive tournaments with per-tier reward payouts.

### Commerce and Stores

Types `Commerce`, `Store`, `StoreDetails`, `Listing`, `ListingDetails`, `Sku`, `SkuDetails`, `OfferDetails`, and `ChainedOffer` represent the Beamable in-game store system, including real-money IAP SKUs, virtual purchase limits, cooldowns, and chained offer sequences triggered by purchases.

### Promotions and Coupons

Types `Promotion`, `PromotionDetails`, `Coupon`, and `CouponDetails` handle time-limited discount campaigns and single- or multi-use coupon codes.

### Scheduling

Types `Schedule` and `ScheduleDetails` provide cron-expression-based scheduling used by stores, events, and promotions.

### Live Events

Types `Event`, `EventDetails`, and `EventContent` model time-limited live events with score submission, per-player ranking, and content-system-backed reward rules.

### Announcements

Types `Announcement` and `AnnouncementDetails` cover platform-wide and audience-targeted broadcasts viewable by players in the client.

### Cloud Save

Types `CloudSave` and `CloudSaveEntry` represent Beamable's key-value persistent storage per player per namespace, suitable for cross-device game state synchronization.

### Stats

Types `Stats` and `StatDetails` model Beamable's flexible player stat system with domain (client/server) and access (public/private) controls.

### Groups

Types `Group`, `GroupDetails`, and `GroupMember` support guilds, clans, and teams with configurable open/approval-based membership and role hierarchy (Leader, Officer, Member).

### Player Mail

Types `Mail` and `MailDetails` represent the in-game mailbox system, including attachment delivery (currencies and items) via `OfferDetails`.

### API Keys

Type `APIKey` covers server-side credential management with scopes and expiry.

## Type Summary

| Category | Types |
|---|---|
| Player | Player, PlayerDetails, PlayerStatus, PlayerInventory |
| Currency | Currency, CurrencyDetails, CurrencyAmount, VirtualCurrency, CurrencyContent |
| Content / Items | ContentItem, ContentDetails, ContentType, Item, ItemDetails, ItemContent |
| Leaderboards | LeaderBoard, LeaderBoardDetails, Ranking, Score, Entry |
| Tournaments | Tournament, TournamentDetails, TournamentStage, TournamentEntry, TournamentChampion, TournamentReward |
| Commerce | Commerce, Store, StoreDetails, Listing, ListingDetails, Sku, SkuDetails, OfferDetails, ChainedOffer |
| Promotions | Promotion, PromotionDetails, Coupon, CouponDetails |
| Scheduling | Schedule, ScheduleDetails |
| Live Events | Event, EventDetails, EventContent |
| Announcements | Announcement, AnnouncementDetails |
| Cloud Save | CloudSave, CloudSaveEntry |
| Session / Auth | Session, SessionDetails, Token, Auth, OAuthDetails |
| Stats | Stats, StatDetails |
| Groups | Group, GroupDetails, GroupMember |
| Mail | Mail, MailDetails |
| API Keys | APIKey |

**Total named types: 66** (excluding scalars, enums, and root operation types)

## References

- Beamable API Reference: https://docs.beamable.com/reference/api-reference
- Beamable Platform Overview: https://docs.beamable.com/docs/beamable-overview
- Beamable GitHub Organization: https://github.com/beamable
