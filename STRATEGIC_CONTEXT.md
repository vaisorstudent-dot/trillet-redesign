# Trillet — Strategic Context & Working Memory

*Captured: 2026-02-28. Conversation between Ori (strategy, US) and AI co-strategist.*
*Purpose: Persistent context that survives compaction. Read this first in any session.*

---

## File Map

| Category | File | Contents |
|----------|------|----------|
| **Company** | [`docs/company/team.md`](docs/company/team.md) | Full team profiles, company size, origin stories |
| **Company** | [`docs/company/traction.md`](docs/company/traction.md) | ARR, pipeline, enterprise proof points, case studies, integrations |
| **Company** | [`docs/company/business_model.md`](docs/company/business_model.md) | Pricing tiers, unit economics, the ask ($5-7M), strategic decisions |
| **VC Research** | [`docs/vc/market_research.md`](docs/vc/market_research.md) | Market sizing, GHL reference, competitor funding, competitive landscape |
| **VC Research** | [`docs/vc/strategic_patterns.md`](docs/vc/strategic_patterns.md) | 10 strategic patterns (platform-of-platforms, lock-in, distribution, etc.) |
| **VC Research** | `docs/vc/build_brief.md` | *Coming — spec for builder agent to create investor artifact* |
| **Project** | [`PROJECT.md`](PROJECT.md) | Master workstream tracker |
| **Prototype** | [`CLAUDE.md`](CLAUDE.md) | Original prototype context (pages, purpose, architecture) |

---

## The Thesis

**Trillet is the platform agencies use to build, brand, and sell AI voice agents — and the infrastructure networks use to deploy them at scale.**

White-label agency voice AI with templating and rebilling on a GHL frame does not exist in the market. Trillet is defining the category, not competing in one.

---

## The Paradigm Shift

### Where We Were (trillet.ai today)
- All segments exist — D2C, Agency, Enterprise, Developer
- **The problem is fragmented, incoherent positioning.** Agency is buried under `/whitelabel`. Enterprise is a generic managed service page. No unifying thesis.

### Where We're Going
- Agency-first GTM. "The GHL of Voice AI."
- 4-tier fractal: Starter ($59) → Agency ($299) → Lite SaaS ($497) → Pro SaaS ($1,497+)
- D2C is a tail. Enterprise narrative is timeline-gated.

### The Shift Is Three Things At Once
1. **Storytelling** — telling existing capabilities correctly
2. **New product layers** — Lite SaaS and Pro SaaS are genuinely new
3. **Enterprise re-architecture** — managed service → scalable API model (though traditional enterprise is still welcome as revenue)

### Timeline-Gated Narrative
- **Phase 1 (Now → 12mo)**: Lead with Agency. Enterprise for inbound only, not actively narrated.
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
2. **AEO works but is fragile.** Zero ad spend, LLMs recommend Trillet. But platform-dependent and not permanently defensible. Window of opportunity.
3. **GHL parallel has limits.** Validates the playbook but GHL has massive community momentum. Trillet's structural advantages: 5-min URL deploy, operational lock-in, templates as full products.
4. **GHL's voice AI feature = market validation, not threat.** They bolted voice onto marketing automation. Voice-as-feature ≠ voice-as-product.

---

## Open Threads

1. **`stitch_workflow`** — Empty file. Ori will explain when ready.
2. **VC investor artifact** — Build brief coming next. All data inputs complete.
3. **Marketplace** — Future vision at scale. Not current priority.
4. **Codebase refactoring** — Plan exists, secondary to strategic work.
5. **Downstream effects of paradigm shift** — Ori has not enumerated all.

---

## The Prototype (this repo)

5 static HTML pages, 1 CSS, 1 JS. Hosted at: https://vaisorstudent-dot.github.io/trillet-redesign/

| Page | Purpose |
|------|---------|
| `index.html` | Dual-audience homepage |
| `agency.html` | Agency pitch |
| `pricing.html` | 4 tiers side-by-side |
| `enterprise.html` | Pro SaaS / Process Configurator |
| `architecture.html` | Internal fractal thesis |

---

*Re-read this file at the start of any new or continued session.*
