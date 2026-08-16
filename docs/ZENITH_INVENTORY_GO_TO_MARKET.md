# Zenith Inventory — Go-to-Market Plan

## Objective

Sell a focused barcode-first inventory product to small industrial businesses without turning Zenith into an unlimited custom-software shop.

The sales motion should become progressively more product-led:

`show product -> let user try -> observe friction -> sell license/setup/integration -> reuse what repeats`

## Initial buyer

Best early-fit businesses:
- small manufacturers
- machine shops
- metal fabricators
- warehouses
- distributors
- maintenance/material stockrooms
- industrial businesses still using spreadsheets/manual tracking for part of inventory

Best early contacts:
- owner
- general manager
- operations manager
- plant manager
- inventory/materials lead
- purchasing/operations person at a small shop

Avoid initially:
- companies requiring enterprise procurement/security review before a pilot
- businesses expecting a full ERP/MRP replacement
- highly regulated/mission-critical deployment where Zenith cannot yet support the risk
- prospects demanding large custom integrations before trying the core product

---

# Launch ladder

## Stage 0 — No selling yet: build founder-usable product

Trigger: Milestones 0–3 in the product repository.

Commercial work:
- maintain the existing prospect pipeline
- collect examples of inventory spreadsheets/workflows when available
- do not mass-pitch an unfinished installer
- prepare product name, basic positioning, and trial language

Primary outcome: Zenith can hand someone an installer rather than source code/setup instructions.

## Stage 1 — Private pilot

Trigger: product Milestone 4 passes.

Target: 3–5 local/qualified businesses or users.

Offer:
> "I built a simple barcode-first inventory tool for smaller industrial operations that do not want a full ERP rollout. I'm looking for a few businesses to try the early Windows version and tell me where it does or doesn't fit."

Pilot should be free or heavily reduced only because the customer is providing structured product feedback. Do not provide unlimited free customization.

Ask the user to do actual tasks:
- install it
- import/enter inventory
- look up/scan items
- receive/consume stock
- check low stock
- back up data

Then ask:
- what was confusing?
- what would stop you using this tomorrow?
- which existing system does it need to exchange data with?
- would you pay for the standard product, setup, or that integration?

## Stage 2 — Paid beta

Trigger: at least one pilot wants to keep using it or requests concrete paid work.

Simple initial offer structure:

### Standard product
Desktop/local Zenith Inventory license.

### Optional paid services
- onboarding/setup
- spreadsheet cleanup/migration
- custom import/export mapping
- external-system integration
- bounded workflow customization
- support/maintenance

Pricing starts as an experiment. The first commercial target is a clear paid transaction and a $500+ customer relationship, not a perfect price book.

## Stage 3 — Repeatable local sales

Trigger: first paid user + stable install/onboarding.

Use:
- existing Zenith manufacturing/industrial prospect pipeline
- direct LinkedIn connections to owners/operations people
- warm referrals from pilot users
- local manufacturing networking/events
- short demo video linked from the Zenith website
- simple product landing/download page

Message changes from generic consulting to product fit:

> "We built Zenith Inventory for smaller industrial teams that need barcode/location/quantity tracking without rolling out a full ERP. If you're still doing part of that in spreadsheets, I can show you the Windows trial."

## Stage 4 — Broader discovery channels

Trigger: stable public release, support process, and credible customer proof/reviews.

Evaluate:
- Capterra/G2 Digital Markets product listing
- Microsoft Store distribution for trusted Windows install/discovery
- Tennessee manufacturing associations and councils
- targeted industrial directories/communities
- partnerships with barcode hardware providers, local IT/MSP firms, or industrial consultants where incentives make sense

Do not spend heavily on paid lead generation until conversion and onboarding economics are known.

---

# Where to find first users

## Tier 1 — Existing local pipeline

Highest priority because research/contact work already exists.

Use the existing Memphis/Tipton/Millington/Covington/Arlington manufacturing prospects. Once the product is pilot-ready, re-approach appropriate contacts with a concrete demo/trial instead of a blank-page automation pitch.

## Tier 2 — Local manufacturing network

Explore the Greater Memphis Chamber's Advanced Manufacturing Council and related manufacturing events/networking as a source of relationships and pilot introductions.

## Tier 3 — Tennessee manufacturing network

Explore the Tennessee Manufacturers Association / Tennessee Chamber for statewide manufacturing relationships, events, and visibility after the trial is credible.

## Tier 4 — Software buyer directories

After public proof, list the product where buyers already research inventory/manufacturing software. Use reviews/testimonials to create credibility before paying aggressively for leads.

## Tier 5 — Windows distribution

After installer/release maturity, evaluate Microsoft Store distribution. The Store can support Win32 applications and can provide a more trusted install/discovery path. Distribution strategy should not delay the first private pilots.

---

# Sales assets required before paid beta

- product name and one-sentence positioning
- working Windows installer
- 2–3 minute demo video
- 5–8 clean screenshots
- one-page feature/limitations page
- quick-start guide
- trial terms
- backup/data-responsibility language
- simple pricing sheet
- onboarding checklist
- integration request worksheet
- support email/contact route

---

# Integration monetization

Treat external-system variation as expected.

When a customer says "we need it to work with X," do not immediately hard-code X into the core.

Classify request:

1. **Core** — nearly every user needs it.
2. **Reusable integration** — system-specific but likely useful to multiple customers.
3. **Customer mapping/customization** — narrow one-off need; price separately.
4. **Out of scope** — too large/risky/unrelated.

For reusable integrations:
- quote implementation separately
- preserve generic adapter contract
- document supported version/format
- create regression tests
- consider selling the adapter as an add-on for future customers

The integration library can become a moat only if it remains modular.

---

# Automation plan

Automate repetitive work before scaling sales volume.

Engineering automation:
- CI test run on push/PR
- automated Windows release build after product packaging is stable
- versioned release artifacts
- regression tests for each reusable integration
- repeatable demo-data creation

Sales/operations automation:
- keep prospect/status records in the Zenith pipeline
- use scheduled follow-up checkpoints rather than relying on memory
- use reusable pilot/onboarding questionnaires
- template proposals and integration scoping
- record feature/integration requests in GitHub issues
- convert repeated requests into roadmap evidence rather than keeping them in chats/notes

Do **not** automate spam outreach. Automation should remove administration, not remove judgment.

---

# Evidence-based product decisions

Every major feature should be tied to at least one of:
- observed user failure
- repeated pilot request
- paid customer requirement
- data integrity/security requirement
- installation/support reduction

A feature does not enter the roadmap merely because a competitor has it.

---

# Commercial scorecard

Track weekly once pilots begin:

| Metric | Target/question |
|---|---|
| Pilot installs attempted | Are real people trying it? |
| Successful self-installs | Can they install without Zach? |
| Primary workflows completed | Scan/search/receive/consume/import/backup |
| Pilot retention | Does anyone want to keep using it? |
| Paid users | Has someone paid? |
| Onboarding hours/customer | Is support burden falling? |
| Integration requests | Which systems repeat? |
| Reusable integrations | Are requests becoming IP? |
| Support defects | What blocks trust? |
| Revenue | License + setup + integrations + support |

## Main sales rule

Do not measure progress only by outreach count. The strongest signal is a qualified business installing the product, using it with representative inventory, and being willing to pay to keep it or connect it to the rest of its operation.
