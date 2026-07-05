# Boardable (boardable)

Boardable is board management software for nonprofits, associations, foundations, and other mission-driven organizations. It covers meeting scheduling, agenda building, a document center, minutes and AI-generated meeting summaries, e-voting, task assignments, groups/committees, member directories, and built-in video conferencing (Boardable Video).

## API Access Model

**Boardable does not publish a documented public developer API.** As of this review (2026-07-05):

- There is **no developer portal** — `developers.boardable.com` and `developer.boardable.com` both redirect to the marketing homepage.
- There is **no published API reference, no OpenAPI definition, no self-serve API keys, and no documented webhooks.**
- A **private, authentication-gated backend API** is observable at `https://api.boardable.com` (for example, `GET https://api.boardable.com/accounts` returns `HTTP 401 Unauthorized`). It powers the Boardable web and mobile apps but is **undocumented** and is **not offered as a public or partner integration surface.**
- Some third-party directory listings describe Boardable as offering an "open API," but **Boardable itself publishes no developer documentation** to substantiate that claim.

Integrations are delivered through **pre-built connectors** rather than a documented API: Salesforce, Microsoft 365 (Teams, Outlook, SharePoint, OneDrive), Google Drive & Calendar, Zoom, Dropbox, LinkedIn, and YouTube.

This entry is therefore an **honest stub**: no APIs are listed in `apis.yml` because none are publicly documented.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/boardable/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/boardable/refs/heads/main/apis.yml)

## Tags

- Board Management
- Governance
- Nonprofit
- Meetings
- Board Portal
- Collaboration
- No Public API

## Timestamps

- **Created:** 2026-07-05
- **Modified:** 2026-07-05

## Plans

Boardable is priced per user, per month, billed annually (about 10% savings vs. monthly):

- **Essentials** — $20.99/user/mo — document center, agenda builder, meeting scheduler, board packets; 1,000 files, 5 guests/meeting, 10 groups.
- **Professional** (most popular) — $29.99/user/mo — adds custom data fields, governance forms, eSignatures, public sites; unlimited files, 10 guests/meeting, 25 groups.
- **Professional+** — $35.99/user/mo — adds AI Meeting Minutes & Transcripts, unlimited surveys, Boardable Video; unlimited files, guests, groups.
- **Enterprise** — custom quote — volume discounts and tailored terms.

A 14-day free trial of Professional features is offered with no credit card required. See [plans/boardable-plans-pricing.yml](plans/boardable-plans-pricing.yml). No API or SSO add-on is documented in Boardable's pricing.

## Common Properties

- [Website](https://boardable.com)
- [LinkedIn](https://www.linkedin.com/company/boardable)
- [Documentation](https://docs.boardable.com/knowledge/getting-started-with-boardable) (end-user help center)
- [Plans](plans/boardable-plans-pricing.yml)

## Review

See [review.yml](review.yml). Boardable exposes no documented public WebSocket API — and no documented public developer API of any kind. The only observable API is a private, auth-gated backend at `https://api.boardable.com` that serves the apps and is not offered for public integration.

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
