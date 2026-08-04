# Boardable (boardable)

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
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
