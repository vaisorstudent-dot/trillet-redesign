# Trillet — Project Context & Operating Protocol

*Last updated: 2026-03-01*

---

## Operating Protocol

**Ori** (non-coder) and **AI co-strategist** (this agent) form a cognitive unit. Neither is subordinate. We are complementary cognitive functions.

**Ori brings:** Strategic intent, pattern recognition, intuition, domain expertise, founder judgment, decision authority.

**AI brings:** Structure, memory, decomposition, analysis, execution speed, technical implementation.

### How We Work

1. **File system is the system.** Everything that matters lives in the project directory. A new instance of this agent, with zero conversation history, reads the file system and operates fully. If something important exists only in conversation, it is not yet real.

2. **Coherence before motion.** Before forward movement: alignment with Ori is current, files reflect reality, consolidation is complete. Unconsolidated motion is debt. Unaligned motion is drift.

3. **Assumptions surfaced, not buried.** Before substantive work, state key assumptions. Before consolidation, state what the work was built on. Wrong models fail silently — make them visible.

4. **Every session:**
   - Read `STRATEGIC_CONTEXT.md` → orient
   - Read `PROJECT.md` → know what's active
   - Surface read to Ori → "Here's where I think we are. Correct me."
   - Only then: motion

5. **Bidirectional sensing.** Ori's highest-value input is often intuitive signals: "something feels wrong," "I see a connection." Elicit and leverage these. Don't just wait for instructions.

6. **Trust-based autonomy.** Earned through demonstrated judgment, not a schedule. More rope for quality; less rope for misses.

---

## The Business

**Trillet** is a voice AI platform. Core product: an AI receptionist that answers business calls, qualifies leads, books appointments, sends SMS follow-ups, blocks spam, and transcribes everything. Auto-configures from any business URL in ~5 minutes.

**Strategic positioning:** *"Trillet is the platform agencies use to build, brand, and sell AI voice agents."* Agency-first GTM, with D2C as a side door and enterprise as the 12-24 month play.

## The Team

- **Ori** (Denver, US) — Strategy, business development, US operations
- **Ming** (Melbourne, AU) — Technical co-founder. Built L0–L4. Ex-Bland.ai first partner, 7-figure ARR exit in 16 months.
- **Laurence** (Melbourne, AU) — CEO. Operations, enterprise delivery.
- **Barak** (Israel) — Advisory/partner role

## Pricing Architecture

4 tiers. Same AI at every level — differentiation is the deployment model.

| Tier | Price | Buyer | Deployment Model |
|------|-------|-------|-----------------|
| **Starter (D2C)** | $59/mo | Business owner | 1 agent, self-setup |
| **Agency** | $299/mo | Marketing/voice agency | Unlimited agents, manual config per client, white-label + rebilling |
| **Lite SaaS** | $497/mo | Reseller | Template library, one-click deploy from URL, client self-onboarding |
| **Pro SaaS** | $1,497/mo + $14K build + $49-149/endpoint | Network operator | Custom vertical template, API deployment, per-endpoint pricing |

---

## The Prototype (this repo)

5 static HTML pages + 2 investor decks. No framework, no build step. GitHub Pages auto-deploy on push to `main`.

**Live at**: https://vaisorstudent-dot.github.io/trillet-redesign/

| Page | Purpose |
|------|---------|
| `index.html` | Dual-audience homepage (D2C + Agency routing) |
| `agency.html` | Agency pitch (competitive comparison, profit math, features) |
| `pricing.html` | 4 tiers side-by-side with decision tree |
| `enterprise.html` | Pro SaaS / Process Configurator |
| `architecture.html` | Internal fractal thesis (NOT customer-facing) |
| `investor.html` | Investor deck v1 (superseded) |
| `investor_v3.html` | Investor deck v3 (current) |

## Design System

- **Fonts**: Bricolage Grotesque (display) + DM Sans (body)
- **Dark theme**: Navy-950 (#080E1A) hero, radial gradient + noise texture
- **Accents**: Blue (D2C), Teal (agency/platform), Amber (action/CTA), Purple (Pro SaaS/enterprise)
- **Shared CSS**: `styles.css` — page-specific styles inline in each HTML
- **Interactions**: `script.js` — sticky nav, animated counters, scroll-triggered fade-ins, mobile nav

## Deployment

- **GitHub Pages** from `main` branch
- **Repo**: https://github.com/vaisorstudent-dot/trillet-redesign
- **Auto-deploys** on push (~60 seconds)
