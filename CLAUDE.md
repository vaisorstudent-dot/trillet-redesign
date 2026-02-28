# Trillet Redesign Prototype — Project Context

## What This Is

A clickable HTML prototype of the redesigned trillet.ai website. 5 static pages (HTML/CSS/JS, no framework, no build step). Built for an internal team presentation to align on brand positioning, information architecture, and tier structure before the technical co-founder (Ming) leaves for China in ~3 weeks.

**Live at**: https://vaisorstudent-dot.github.io/trillet-redesign/

## The Business

**Trillet** is a voice AI platform. The core product: an AI receptionist that answers business phone calls, qualifies leads, books appointments, sends SMS follow-ups, blocks spam, and transcribes everything. It auto-configures from any business URL in ~5 minutes — no manual data entry.

The strategic positioning (decided during this prototype process): **"Trillet is the platform agencies use to build, brand, and sell AI voice agents."** Agency-first GTM, with D2C as a side door and enterprise as the 12-24 month play.

## The Team

- **Ori** (US) — Strategy, business development, US operations. The person commissioning this prototype.
- **Ming** (AU) — Technical co-founder. Built the core AI, the agent builder, the agency platform (white-label, sub-accounts, rebilling). Also designed the enterprise deployment architecture (Process Configurator). Thinks visually — this prototype exists because a document wouldn't land.
- **Laurence** (AU) — Operations.
- **Barak** — Advisory/partner role.

## The Pricing Architecture

4 tiers. Same AI at every level — differentiation is the deployment model, not the agent quality.

| Tier | Price | Buyer | Deployment Model |
|------|-------|-------|-----------------|
| **Starter (D2C)** | $59/mo | Business owner | 1 agent, self-setup |
| **Agency** | $299/mo | Marketing/voice agency | Unlimited agents, manual config per client, white-label + rebilling |
| **Lite SaaS** | $497/mo | Reseller | Template library, one-click deploy from URL, client self-onboarding |
| **Pro SaaS** | $1,497/mo + $14K build + $49-149/endpoint | Network operator | Custom vertical template, API deployment, per-endpoint pricing |

**Key decisions already locked:**
- D2C price is $59 (locked by Ori)
- Rebilling available at ALL agency tiers ($299+), not gated behind $497. The closing question from their best lead was "can I invoice my clients?" — gating rebilling kills the flywheel.
- Tier differentiation is deployment model: manual → template → API. Not feature gates on call quality.
- Per-endpoint pricing (not revenue share, not flat fee) for Pro SaaS. Eliminates rev-share bypass risk and scales with the network.

## Key Strategic Concepts

### The Fractal / Atomic Unit
Every product Trillet sells is the same atomic unit (one voice AI agent) at different deployment scales. A $59 D2C agent and a $99/endpoint enterprise agent run identical AI. The architecture page (`architecture.html`) visualizes this.

### The GHL Parallel
GoHighLevel (GHL) is a $2B+ marketing automation platform that grew via agency white-labeling. Trillet follows the same playbook (white-label, SaaS mode, sub-accounts, snapshots/templates, community) but has structural advantages: 5-min deployment from URL (GHL requires manual setup), operational lock-in (switching off Trillet = calls go unanswered), and templates that are full working products (not just config exports).

### AEO (AI Engine Optimization)
Trillet's #1 acquisition channel is LLMs recommending them. Zero ad spend. A real customer spent an hour interrogating ChatGPT about every voice AI platform; ChatGPT recommended Trillet as #1. The site content is structured to be LLM-retrievable.

### Process Configurator
Ming's enterprise architecture: custom agent build → snappable template → one-click API deployment across networks. This is the Pro SaaS unlock. Example: one dental network template deploys to 25+ clinics via API, each agent auto-configuring from the clinic's website. The Mark/Nexit deal ($14K implementation) is the proof-of-concept.

### Operational Lock-in
Unlike marketing SaaS (easily switchable), Trillet handles live inbound calls. Switching off means calls go unanswered until a replacement is configured and tested at every endpoint. Switching cost scales linearly with the number of endpoints. At 100+ endpoints, it's effectively permanent — no contract needed.

## The Prototype — What's In Each Page

### `index.html` — Homepage
Dual-audience routing. Hero: "Never miss a call again. Or let your clients say the same." Two route cards (D2C blue / Agency teal). Two-track "how it works" on dark background. Mock call transcript (plumber emergency). Mock ChatGPT conversation showing Trillet recommendation (real customer journey). 6 capability cards. Industry tags. Dual testimonials. Triple CTA.

### `agency.html` — Agency Pitch
Leads with competitive comparison (vs Retell, Vapi, Synthflow) + deploy mockup. The math (3 profit scenarios at 10/25/50 clients). 6 feature cards. 3 agency tier cards with "Best for:" context. FAQ handling real objections ("What if my clients don't like the AI?"). CTA: "The GHL of voice AI."

### `pricing.html` — All 4 Tiers
Side-by-side pricing cards. "Recommended" badge on Lite SaaS. Decision tree ("Answer one question" → routes to correct tier). Comparison table grouped by category (Scale, Branding, Deployment, Support) — universal features stated once in intro, not repeated as rows. FAQ covers the real confusion points (Agency vs Lite SaaS, what's in the $14K build).

### `enterprise.html` — Pro SaaS / Process Configurator
4-step numbered process flow (build → template → API → deploy). Dental network case study with concrete metrics (25 clinics, 1 week, 4,200+ calls/mo). Economics: cost vs revenue side-by-side with honest disclaimers. "vs the old way" comparison ($60-70K custom build → $14K template). Vertical tag cloud. Timeline (discovery → build → API → rollout in ~3 weeks). Compliance badges with practical descriptions.

### `architecture.html` — Internal Team Visualization
**NOT customer-facing.** Amber "INTERNAL" banner. Visualizes: the atomic agent unit, the fractal (4 scales with nesting), nested enterprise (dental network org tree with pulse dots), the infrastructure stack (L0-L4 with live/building/planned status), the GHL parallel (where it holds, where Trillet breaks it), the flywheel (AEO loop + marketplace loop), vertical lock-in dynamics, and 0-12mo / 12-24mo strategic roadmap.

## Design System

- **Fonts**: Bricolage Grotesque (display) + DM Sans (body)
- **Dark theme**: Navy-950 (#080E1A) hero/dark sections, radial gradient + noise texture
- **Accents**: Blue (D2C), Teal (agency/platform), Amber (action/CTA/agency highlight), Purple (Pro SaaS/enterprise)
- **Shared CSS**: `styles.css` — all page-specific styles are inline in each HTML file
- **Interactions**: `script.js` — sticky nav, animated counters, scroll-triggered fade-ins, mobile nav toggle

## Deployment

- **GitHub Pages** from `main` branch (legacy deploy mode)
- **Repo**: https://github.com/vaisorstudent-dot/trillet-redesign
- **Auto-deploys** on push to `main` (~60 seconds)
- No build step — pure static files

## What's NOT Decided / Still Open

- Exact per-minute call usage rates and how they display on the site
- Whether the template marketplace is in scope for the current roadmap discussion
- Community/certification program details
- Real testimonial attribution (current testimonials are representative but some are placeholder personas)
- Whether the "Architecture" nav link stays after the team presentation or gets removed for public launch
- Production domain and hosting (this is a prototype on GitHub Pages, not the final deployment)
