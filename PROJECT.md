# Trillet — Master Project File

*Last updated: 2026-02-28*

## Workstreams

| # | Workstream | Status | Priority |
|---|-----------|--------|----------|
| 1 | **VC / Investor Artifact** | 🔨 Active — all inputs complete, build brief next | **High** |
| 2 | **Stitch Workflow** | ⏳ Pending Ori context | TBD |
| 3 | **Codebase Refactoring** | 🅿️ Parked | Low |
| 4 | **Architecture Page Corrections** | Absorbed into VC workstream | — |

---

## Workstream 1: VC / Investor Artifact

**Goal:** Standalone investor-grade HTML artifact (separate from architecture.html). A different builder agent executes from a build brief we produce.

### Data Inputs — ALL COMPLETE ✅
| Input | Status | Location |
|-------|--------|----------|
| Team profiles | ✅ | `docs/company/team.md` |
| Traction & case studies | ✅ | `docs/company/traction.md` |
| Business model & unit economics | ✅ | `docs/company/business_model.md` |
| Market sizing & competition | ✅ | `docs/vc/market_research.md` |
| Strategic patterns (10) | ✅ | `docs/vc/strategic_patterns.md` |
| The ask ($5-7M Seed+) | ✅ | `docs/company/business_model.md` |

### Next Steps
- [ ] Write build brief for builder agent (`docs/vc/build_brief.md`)
- [ ] Builder agent executes → `investor.html`
- [ ] Review & iterate

---

## Workstream 2: Stitch Workflow
*Pending context from Ori. Empty file at `stitch_workflow`.*

## Workstream 3: Codebase Refactoring
*Parked — prototype serves current purpose.*

---

## File Structure

```
STRATEGIC_CONTEXT.md      ← Lean thesis + file map (start here)
PROJECT.md                ← This file (workstream tracker)
CLAUDE.md                 ← Original prototype context
docs/
  company/
    team.md               ← Team profiles, origin stories
    traction.md           ← ARR, case studies, enterprise proof points
    business_model.md     ← Pricing, unit economics, the ask
  vc/
    market_research.md    ← TAM/SAM, GHL reference, competitors
    strategic_patterns.md ← 10 strategic patterns
    build_brief.md        ← Coming next
```
