# Trillet — Master Project File

*Last updated: 2026-03-01*

## Workstreams

| # | Workstream | Status | Priority |
|---|-----------|--------|----------|
| 1 | **VC / Investor Artifact** | 🔨 Active — v3 built, critiqued, decisions surfaced | **High** |
| 2 | **Orchestrator System** | ✅ Operational — file system restructured | **High** |
| 3 | **Stitch Workflow** | ✅ Documented — ready to apply | Medium |
| 4 | **Codebase Refactoring** | 🅿️ Parked | Low |

---

## Workstream 1: VC / Investor Artifact

**Goal:** Standalone investor-grade HTML artifact for seed+ raise ($5–7M).

### Completed
- [x] All data inputs gathered (team, traction, business model, market research, strategic patterns)
- [x] Build brief written → executed → `investor.html` (v1) → **deleted** (superseded)
- [x] Iterated to `investor/deck_v3.html` (current version)
- [x] VC critique panel run → `docs/vc/critique_vc_panel.md` (4-agent evaluation)
- [x] SaaS consulting panel run → `docs/vc/saas_assessment.md` (5-agent, 60K words)
- [x] Key decisions extracted → `docs/vc/decisions_needed.md` (6 decisions for founding team)

### Open / Pending Ori + Team
- [ ] **Decision 1:** Lead with enterprise or agency-first? (Rec: enterprise-led, agency-seeded)
- [ ] **Decision 2:** D2C channel conflict position
- [ ] **Decision 3:** 20-client cap on Agency tier ($299)
- [ ] **Decision 4:** Crisp answer for "why isn't Ming CEO?"
- [ ] **Decision 5:** Raise $5M or $7M? (Rec: $7M)
- [ ] **Decision 6:** First US hire timing and profile
- [ ] **Blocker:** One agency case study with real metrics (before deck goes out)
- [ ] **Blocker:** Update trillet.ai to match deck pricing ($59, not $29)
- [ ] Deck v4 incorporating all fixes

### Artifacts

| File | Purpose | Status |
|------|---------|--------|
| `investor/deck_v3.html` | Investor deck v3 (current) | Active — needs fixes from critique |
| `docs/vc/critique_vc_panel.md` | VC evaluation panel output | Complete |
| `docs/vc/saas_assessment.md` | Full SaaS advisory assessment | Complete |
| `docs/vc/decisions_needed.md` | 6 decisions for founding team | **Awaiting team decisions** |
| `docs/vc/market_research.md` | TAM/SAM, GHL reference, competitors | Complete |
| `docs/vc/strategic_patterns.md` | 10 strategic patterns | Complete |

---

## Workstream 2: Orchestrator System

**Goal:** Operationalize the distributed cognition architecture as the working protocol for Ori + AI co-strategist.

### Completed
- [x] `system/SYSTEM.md` written — governing principles, cognitive motion, file system design
- [x] `system/ORCHESTRATOR_PROMPT.md` written — thinned to boot sequence
- [x] Operationalization plan approved by Ori
- [x] File system consolidated — all files reflect reality
- [x] `CLAUDE.md` restructured — encodes operating protocol
- [x] File system restructured — `system/`, `investor/`, `workflows/` created, taxonomy follows problem spaces

### System Files

| File | Purpose | Authority |
|------|---------|-----------|
| `system/SYSTEM.md` | Living design document | Design intent |
| `system/ORCHESTRATOR_PROMPT.md` | Boot sequence | Operational behavior |
| `system/STATE.md` | Live state tracker | Active motion, assumptions, alignment |
| `CLAUDE.md` | Agent governance instructions | Behavioral directives |
| `STRATEGIC_CONTEXT.md` | Cold-start entry point + file map | Orientation |
| `PROJECT.md` | This file — workstream tracker | Current state |

---

## Workstream 3: Stitch Workflow

**Goal:** Design-first build workflow (Decide → Research → Blueprint → Design → Build + Validate).

**Status:** Full workflow documented in `workflows/stitch.md`. Not yet applied to a problem space. Ready to use when building or redesigning pages.

---

## Workstream 4: Codebase Refactoring

**Status:** Parked. Prototype serves current purpose (5 static HTML pages, working on GitHub Pages).

---

## File Structure

```
# Entry Points (root)
STRATEGIC_CONTEXT.md               ← Cold-start: read first
PROJECT.md                         ← This file (workstream tracker)
CLAUDE.md                          ← Operating protocol + project context

# System Architecture
system/
  SYSTEM.md                        ← Design intent (orchestrator architecture)
  ORCHESTRATOR_PROMPT.md           ← Boot sequence for orchestrator agent
  STATE.md                         ← Live state: motion, assumptions, alignment

# Investor Workstream
investor/
  deck_v3.html                     ← Current investor deck

# Company & VC Research
docs/
  company/
    team.md                        ← Team profiles, origin stories
    traction.md                    ← ARR, case studies, enterprise proof points
    business_model.md              ← Pricing, unit economics, the ask
  vc/
    market_research.md             ← TAM/SAM, GHL reference, competitors
    strategic_patterns.md          ← 10 strategic patterns
    critique_vc_panel.md           ← VC evaluation panel (4-agent)
    saas_assessment.md             ← Full SaaS advisory panel (5-agent, 60K words)
    decisions_needed.md            ← 6 decisions for founding team

# Prototype (GitHub Pages — must stay in root)
index.html                         ← Dual-audience homepage
agency.html                        ← Agency pitch
pricing.html                       ← 4 tiers side-by-side
enterprise.html                    ← Pro SaaS / Process Configurator
architecture.html                  ← Internal fractal thesis (not customer-facing)
styles.css                         ← Shared CSS
script.js                          ← Shared JS

# Workflows
workflows/
  stitch.md                        ← Design-first build workflow
```
