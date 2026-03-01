# Trillet — Strategic Context & Working Memory

*Last updated: 2026-03-01. Ori + AI co-strategist.*
*Purpose: Cold-start entry point. Read this first in any session.*

---

## File Map

| Category | File | Contents |
|----------|------|----------|
| **System** | [`system/SYSTEM.md`](system/SYSTEM.md) | Orchestrator architecture — governing principles, cognitive motion, design intent |
| **System** | [`system/ORCHESTRATOR_PROMPT.md`](system/ORCHESTRATOR_PROMPT.md) | Boot sequence for orchestrator agent |
| **System** | [`CLAUDE.md`](CLAUDE.md) | Operating protocol + project context |
| **Project** | [`PROJECT.md`](PROJECT.md) | Master workstream tracker — **check this for current state** |
| **Company** | [`docs/company/team.md`](docs/company/team.md) | Full team profiles, 20 people, 4 founders, origin stories |
| **Company** | [`docs/company/traction.md`](docs/company/traction.md) | $500K ARR, enterprise proof points, case studies, integrations |
| **Company** | [`docs/company/business_model.md`](docs/company/business_model.md) | 4 tiers, unit economics, the ask ($5-7M), locked decisions |
| **VC Research** | [`docs/vc/market_research.md`](docs/vc/market_research.md) | TAM/SAM, GHL reference, competitive landscape |
| **VC Research** | [`docs/vc/strategic_patterns.md`](docs/vc/strategic_patterns.md) | 10 strategic patterns (platform-of-platforms, lock-in, distribution, etc.) |
| **VC Critique** | [`docs/vc/critique_vc_panel.md`](docs/vc/critique_vc_panel.md) | VC evaluation panel — 4-agent critique of investor deck |
| **VC Critique** | [`docs/vc/saas_assessment.md`](docs/vc/saas_assessment.md) | Full SaaS advisory panel — 5-agent, 60K-word assessment |
| **VC Critique** | [`docs/vc/decisions_needed.md`](docs/vc/decisions_needed.md) | 6 key decisions for founding team before deck goes out |
| **Investor** | [`investor/deck_v3.html`](investor/deck_v3.html) | Current investor deck (v3) |
| **Prototype** | HTML files in root | 5 pages, live at GitHub Pages |
| **Workflow** | [`workflows/stitch.md`](workflows/stitch.md) | Design-first build workflow (Decide→Research→Blueprint→Design→Build) |

---

## The Thesis

**Trillet is the platform agencies use to build, brand, and sell AI voice agents — and the infrastructure networks use to deploy them at scale.**

White-label agency voice AI with templating and rebilling on a GHL frame does not exist in the market. Trillet is defining the category, not competing in one.

---

## Current State (as of 2026-03-01)

**Active motion:** File system restructured. Orchestrator operationalized. VC workstream blocked on team decisions.

**VC workstream:** Investor deck v3 (`investor/deck_v3.html`) complete. Two critique panels run. Six decisions surfaced for founding team (`docs/vc/decisions_needed.md`). **Blocked on team decisions before deck goes to investors.** Key blockers: one agency case study, updated trillet.ai pricing, and the enterprise-vs-agency framing decision.

**Orchestrator system:** Live. File system consolidated and restructured. Operating protocol encoded in `CLAUDE.md`. System architecture in `system/`.

---

## The Paradigm Shift

### Where We Were (trillet.ai today)
- All segments exist — D2C, Agency, Enterprise, Developer
- Fragmented, incoherent positioning. Agency is buried under `/whitelabel`. Enterprise is a generic managed page.

### Where We're Going
- Agency-first GTM. "The GHL of Voice AI."
- 4-tier fractal: Starter ($59) → Agency ($299) → Lite SaaS ($497) → Pro SaaS ($1,497+)
- D2C is a tail. Enterprise narrative is timeline-gated.

### The Shift Is Three Things At Once
1. **Storytelling** — telling existing capabilities correctly
2. **New product layers** — Lite SaaS and Pro SaaS are genuinely new
3. **Enterprise re-architecture** — managed service → scalable API model

### Timeline-Gated Narrative
- **Phase 1 (Now → 12mo)**: Lead with Agency. Enterprise for inbound only.
- **Phase 2 (12-24mo)**: Layer in enterprise as L4 proves out.
- **Investor narrative shows both phases. Public website shows Phase 1 only.**

---

## Infrastructure Stack

| Layer | What | Status |
|-------|------|--------|
| L0 | Core AI Engine | ✅ Live |
| L1 | Agent Builder (URL → agent in 5 min) | ✅ Live |
| L2 | Agency Platform (white-label, sub-accounts, rebilling) | ✅ Live |
| L3 | Template Engine (snap → freeze → stamp copies) | ✅ Live |
| L4 | API Distribution / Process Configurator | 🟢 Pilot deployed ("Comms") |

**L3 unlocks Lite SaaS. L4 unlocks Pro SaaS.**
**Investor frame:** "We didn't raise to build the product. We built it. Now we're raising to capture the market."

---

## Non-Trivial Strategic Observations

1. **Operational lock-in is the strongest card.** Switching off = calls go unanswered everywhere. At 100+ endpoints = effectively permanent.
2. **AEO works but is fragile.** Zero ad spend, LLMs recommend Trillet. Platform-dependent and not permanently defensible. Window of opportunity.
3. **GHL parallel has limits.** Validates the playbook but GHL has massive community momentum. Trillet's structural advantages: 5-min URL deploy, operational lock-in, templates as full products.
4. **GHL's voice AI feature = market validation, not threat.** They bolted voice onto marketing automation. Voice-as-feature ≠ voice-as-product.
5. **The competitive window is 9-15 months, not 18-24.** Synthflow ($30M Accel Series A) is the existential threat. Must have 100+ active agencies before they ship white-label features.

---

## Open Threads

1. **6 team decisions** — pricing, positioning, org. See `docs/vc/decisions_needed.md`
2. **Agency case study** — blocker for investor deck. Ori needs to extract from best of ~14 paying agencies.
3. **trillet.ai update** — live site contradicts deck ($29 vs $59, missing tiers)
4. **Stitch workflow** — documented in `workflows/stitch.md`, not yet applied to a problem space
5. **Marketplace** — future vision at scale, not current priority
6. **Codebase refactoring** — parked

---

*Re-read this file at the start of any new or continued session.*
