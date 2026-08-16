# Zenith Capital Group — First 90 Days

This execution plan is now centered on **turning the existing inventory application into a streamlined, trial-ready industrial product** rather than relying primarily on open-ended custom consulting.

The operating loop is:

> Build -> simplify -> package -> put in front of real users -> learn -> sell -> modularize what repeats.

## Operating Rules

- Product work must move the software closer to being installable and usable by a stranger.
- Do not add features simply because they are technically interesting.
- Keep the inventory core small; factory-specific software belongs behind integration/adaptor boundaries.
- Customer contact remains required, but use a concrete product/trial whenever possible instead of blank-page consulting discovery.
- FamiliarVoice continues through bounded milestones and is not abandoned.
- Career Command Center remains internal-first until the workflow is proven enough to justify commercialization.
- No new speculative product becomes active without an explicit decision to pause something else.
- Protect sleep, exercise, food, and recovery because founder capacity is a business asset.

---

# Days 1–14 — Secure, Baseline, and Unbloat

## Zenith Inventory

- [ ] Remove active committed secrets/default credentials from the repository.
- [ ] Rotate any credential that was ever real or reused elsewhere.
- [ ] Create a clean productization branch.
- [ ] Document current valuable behavior before deleting legacy code.
- [ ] Define a smoke-test checklist for inventory CRUD, barcode lookup, quantity adjustment, import/export, labels, backup, and restore.
- [ ] Identify Environmental Pneumatics-specific code and separate it into three groups:
  - useful generic inventory behavior
  - optional manufacturing behavior
  - obsolete/legacy behavior to remove
- [ ] Define the new generic item model.
- [ ] Define an integration interface so ProNest becomes the first adapter rather than a core dependency.
- [ ] Get the current application running on the founder's PC from a clean setup and record every friction point.

**Exit criterion:** we understand exactly what the current program does, what must survive, and what should leave the core.

---

# Days 15–35 — Zero-Hassle Local MVP

Goal: eliminate the current installation burden.

- [ ] Introduce an embedded local database option; SQLite is the first architecture to evaluate.
- [ ] Automatically create the local database/schema on first launch.
- [ ] Store application data in a normal writable user-data directory.
- [ ] Remove PostgreSQL as a requirement for the first single-user desktop release.
- [ ] Package a Windows executable/installer.
- [ ] Add optional fictional demo inventory.
- [ ] Verify install -> launch -> close -> reopen -> backup -> restore on a clean Windows environment.
- [ ] Establish simple versioning and release notes.

**Acceptance target:** a nontechnical user can download/install, launch, and begin entering/importing inventory in under five minutes without Python, PostgreSQL, or a terminal.

---

# Days 36–55 — Streamlined Industrial Inventory Core

Build only the core workflow that most target users need.

- [ ] Generic item fields: SKU/barcode, item name/description, category/material, quantity, unit, location/bin/shelf, minimum stock, supplier, notes, last updated.
- [ ] Optional manufacturing fields: thickness/gauge, dimensions, grade/material details.
- [ ] Fast barcode scan -> lookup -> receive/consume/adjust.
- [ ] Inventory movement/history log.
- [ ] Low-stock/reorder view.
- [ ] Search/filter/sort for hundreds or thousands of items.
- [ ] CSV/XLSX import with validation/preview.
- [ ] CSV/XLSX export.
- [ ] Printable barcode/QR labels.
- [ ] Reliable backup/restore.
- [ ] Basic dashboard: low stock, recent activity, items by location/category.
- [ ] Remove or isolate legacy controls that do not support the primary workflow.

**Exit criterion:** the application feels like one coherent inventory product, not a collection of EP-era utilities.

---

# Days 56–65 — Modular Integrations

The core should not know how every factory operates.

- [ ] Create a stable integration/adaptor contract.
- [ ] Move ProNest-specific transformation/export logic into its own adapter.
- [ ] Keep standard spreadsheet interchange in the core.
- [ ] Define configuration/metadata an adapter can expose to the UI.
- [ ] Create a template/example adapter for future customer systems.
- [ ] Document how a new integration can consume inventory data and produce/import external data without modifying core inventory logic.

Potential future adapters should be driven by actual demand:

- ProNest
- laser/CNC systems
- ERP exports/imports
- accounting systems
- supplier systems
- customer-specific CSV mappings
- APIs

**Architecture rule:** one customer's external system should not permanently bloat the product core.

---

# Days 66–75 — Trial-Ready Release

- [ ] Neutral Zenith product branding.
- [ ] Signed/versioned release build where practical.
- [ ] Download page/release artifact.
- [ ] Fictional industrial demo dataset.
- [ ] Two-to-three-minute demo video or GIF.
- [ ] One-page quick-start guide.
- [ ] Clear feedback/bug-report route.
- [ ] Basic terms around backups, data responsibility, and trial use.

**Exit criterion:** we can send a business one link and reasonably ask them to try the product themselves.

---

# Days 76–90 — Real User Validation and First Revenue

Put the trial in front of **3–5 qualified industrial businesses/users**.

The contact goal is no longer generic mass prospecting. The goal is to get relevant people through a concrete product experience.

Observe:

- Could they install without help?
- Could they import or enter representative inventory?
- Did barcode/quantity workflows make sense?
- Which current system do they need to exchange data with?
- What blocked adoption?
- Which requested features repeat across users?
- Would they pay for the product itself?
- Would they pay for onboarding/data migration?
- Would they pay for a required integration?

### First monetization experiments

Test combinations of:

- local/desktop license
- onboarding and spreadsheet migration
- paid integration modules
- bounded customization
- support/maintenance

Do not build cloud sync, multi-user architecture, purchase orders, MRP, or large SaaS infrastructure merely because they might someday be useful. Those become roadmap items when evidence justifies them.

---

# FamiliarVoice During the 90 Days

FamiliarVoice remains active, but bounded.

- Maintain a clearly defined next milestone.
- Do not allow it to derail the inventory trial-ready sequence.
- Move it toward outside-user testing rather than endless internal polishing.
- Reassess commercialization once Zenith Inventory reaches a stable trial milestone or if FamiliarVoice shows stronger external traction first.

---

# Customer Outreach During the 90 Days

Keep the existing local industrial pipeline and follow-up commitments.

However, shift the purpose of new outreach from:

> "What manual process can I build software for?"

Toward:

> "I built a simple barcode-first inventory tool for small industrial teams. Can you try it and tell me what prevents it from fitting your operation?"

This preserves customer evidence while matching Zenith's product-first strategy.

---

# Revenue Milestones

1. **$1** — proof someone will pay Zenith.
2. **$500** — proof of a real commercial transaction.
3. **First paid product/setup/integration customer** — proof the inventory thesis can monetize.
4. **$1,000/month** — meaningful contribution to personal burn.
5. **$3,000/month** — conservative personal-spending coverage.
6. **$5,000+/month** — room to reinvest.
7. **Stable recurring cash flow** — prerequisite for serious hiring and acquisition planning.

---

# Day-90 Decision

Choose based on evidence:

### A — Double down on Zenith Inventory
Use when businesses can successfully trial it and at least some show willingness to pay for the product, setup, or integrations.

### B — Refine positioning/workflow
Use when users engage with the trial but the product solves the wrong slice of inventory or needs a narrower industrial niche.

### C — Product-plus-services hybrid
Use when the core product creates conversations but most revenue initially comes from migration, integrations, or bounded customization.

### D — Reallocate product priority
Use only if real evidence shows another owned product, such as FamiliarVoice, has materially stronger commercial pull.

The goal is not to defend a favorite idea forever. The goal is to build owned software that real users can adopt and pay for.
