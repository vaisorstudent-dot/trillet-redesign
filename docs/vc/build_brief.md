# VC Investor Artifact — Build Brief

*For: Builder agent*
*Created: 2026-02-28 by Ori Vaisbort + AI co-strategist*
*Output: `investor.html` — standalone, single-file HTML (inline CSS/JS)*

---

## What This Is

A standalone, scroll-driven investor briefing page for Trillet AI. Not a pitch deck. Not the architecture page. A purpose-built investor narrative with real data, premium aesthetics, and strategic depth.

**Target audience:** Seed/Pre-A investors seeing Trillet for the first time.
**Assume:** Zero prior knowledge of Trillet, GHL, or voice AI agency models.
**Tone:** Confident, precise, understated. Not salesy — infrastructure-grade.

---

## Design Direction

### Aesthetic
- **Dark theme.** Deep slate/charcoal background. Not pure black.
- **Stripe-clean, not GHL-busy.** Infrastructure feel, not agency-tool feel.
- **Typography:** Modern sans-serif (Inter or similar from Google Fonts). Clean hierarchy.
- **Accent palette:** Teal (primary — matches existing brand), amber (secondary for highlights/data), indigo (tertiary for vision sections).
- **No stock photos, no illustrations.** Data, diagrams, and typography only.

### Interactions
- **Scroll-driven reveal.** Sections fade/slide in as they enter viewport.
- **Animated counters.** Key metrics ($338K, 0.89%, $500K ARR) count up on scroll.
- **Interactive fractal diagram.** Tiers are hoverable/clickable — show deployment model details.
- **GHL comparison table.** Clean grid with status badges (Shipped / Live / Pilot / Planned).
- **Smooth scroll.** Anchor navigation at top for jumping between sections.

### Structure
- **Single file.** All CSS and JS inline. No external dependencies except Google Fonts.
- **Mobile-first.** VCs read links on phones. Every section must work at 375px.
- **"Confidential" header.** Sticky top bar: *"Trillet AI — Confidential Investor Briefing — February 2026"*
- **No navigation to the prototype site.** This is a standalone document.

---

## Narrative Arc — Section by Section

### Section 1: The Hook (5 seconds)

**Goal:** Stop the scroll. Create "tell me more" urgency.

**Content — cold open, no preamble:**
> A Fortune 500 telecom deployed our voice AI at 25 locations. They're expanding nationally.
>
> Our AI collected $338,000 for a debt collection firm — with a 0.89% call abandonment rate. Industry average: 8–10%.
>
> We built this with 20 people and $0 in external funding.

**Design:** Full-viewport dark section. Text appears with subtle typewriter or fade animation. Numbers animate on scroll. No logo yet — just the statement.

Trillet logo + "Confidential Investor Briefing" appears AFTER the hook, as the user scrolls down.

---

### Section 2: The Gap (why this matters)

**Goal:** Establish the market opportunity without jargon.

**Content — three beats:**

**Beat 1 — The market is real:**
Voice AI market: $6.8B (2025) → $32.6B (2033). 21.5% CAGR.
*(Source: Markets and Markets, Grand View Research)*

**Beat 2 — Everyone is building the wrong thing:**
Bland AI ($65M raised), Vapi ($20M, $130M valuation), Retell ($5M), Synthflow ($20M) — they all built developer tools. APIs for engineers who want to build voice AI from scratch.

But the $6.8B market isn't developers. It's the 50,000+ agencies and service businesses that need to DEPLOY voice AI for their clients — without writing code, without hiring engineers.

**Beat 3 — The GHL proof point:**
GoHighLevel understood this for marketing automation. They built a white-label platform that let agencies resell CRM, funnels, and SMS under their own brand. Result: 2M+ businesses on platform, 781% revenue growth, Inc. 5000 #516, valued at $2B+.

Voice AI has no equivalent. **We're building it.**

**Design:** Clean three-column or vertical flow. Market size number is large and animated. Competitor logos or names in a subtle grid with their funding amounts. GHL stats in a callout box.

**Jargon note:** GHL must be self-explanatory from context. Never assume the reader knows what GoHighLevel is.

---

### Section 3: The Origin Story (why us)

**Goal:** Founder-market fit. Show this team LIVED the gap.

**Content:**

Ming Xu was Bland.ai's first partner — the first person to build a voice AI agency practice on top of the leading infrastructure. He scaled it to 7-figure ARR in 16 months. Then exited.

Why? Because the tooling agencies need doesn't exist. White-label? No. Rebilling? No. Templates? No. One-click deployment? No. Every agency hits the same ceiling: manually configuring agents one by one.

Ming didn't predict the category. He lived the gap. Then he built the platform to fill it.

**Team grid (4 founders):**
- **Laurence Latin** — CEO. Head of Software at Australia's leading healthcare SaaS (Cloudburst). Infrastructure at Dimension Data, Commonwealth Bank. Mission-critical systems.
- **Ming Xu** — COO. Bland.ai's first partner → 7-fig ARR exit. Serial entrepreneur ($5MM+ bootstrapped). Director of Technology at Zeroth Capital (+$35.7M turnover).
- **Ori Vaisbort** — Managing Partner, US. Enterprise infrastructure (IAM for Visa, Check Point Software). 11-year operator. Red Hat Certified Engineer.
- **Barak Blatman** — Managing Partner. Former COO of social platforms (Whiplr, Vigr). Israel Security Agency. B2C product + data expertise.

**Below team:** "20 people. 15 engineers. $0 raised. L0 through L4 built and deployed."

**Design:** Ming's origin story as a brief narrative paragraph (not a bio dump). Team as a 4-up grid with name, title, one-line proof point each. The "$0 raised" line is a standalone callout.

---

### Section 4: The Product (the fractal)

**Goal:** Show the architecture elegance without jargon.

**Header:** "One product. Every scale."

**Content:**

**The core agent (don't call it "atomic unit"):**
Visual flow: Business URL → Web scrape → Agent config → Voice AI → Live agent. Capabilities underneath: call handling, lead qualification, calendar booking, SMS, spam detection, transcripts, 32 languages, CRM sync.

**Key line:** "A $59/month solo operator and a Fortune 500 telecom run the same AI. Only the deployment wrapper changes."

**Four scales (don't call them "fractal tiers" — call them deployment models):**

| Scale | What happens | Who | Price |
|-------|-------------|-----|-------|
| Starter | 1 operator sets up 1 agent for their own business | Solo operators | $59/mo |
| Agency | 1 operator configures agents for each client. White-label + rebilling. | Marketing agencies | $299/mo |
| Lite SaaS | 1 operator deploys from a template library. Clients self-onboard. One click. | Agencies scaling past 15 clients | $497/mo |
| Pro SaaS | Custom template + API. Entire network auto-configures from local context. | Network operators, enterprise | $1,497/mo + $14K build |

**Interactive visualization:** Show each tier nested inside the next (indented or nested boxes). Each tier is hoverable — reveals the deployment model detail. Animate the expansion from Starter → Agency → Lite SaaS → Pro SaaS.

**The insight line (big, centered):**
"Each tier is an order of magnitude more distribution per customer."
1 Starter = 1 endpoint. 1 Agency = 10-50. 1 Lite SaaS = 100+. 1 Pro SaaS = 1,000+.

**Design:** The fractal visualization is the crown jewel. Adapt the existing `architecture.html` nesting but polish it — cleaner lines, hover states, mobile-friendly.

---

### Section 5: Infrastructure Stack

**Goal:** Show product maturity. "We built it. All of it."

**Header:** "Five layers. All live."

**Visual:** Horizontal stacked bars or layered blocks, each lit green (live) or amber (pilot).

| Layer | Name | What it unlocks | Status |
|-------|------|----------------|--------|
| Core AI Engine | Voice processing, NLU, TTS, 32 languages | The intelligence | ✅ Live |
| Agent Builder | URL → live agent in 5 minutes | The magic | ✅ Live |
| Agency Platform | White-label, sub-accounts, Stripe rebilling | The distribution model | ✅ Live |
| Template Engine | Snap → freeze → one-click stamp | The scale unlock | ✅ Live |
| API Distribution | REST API, auto-configure, per-endpoint billing | The infrastructure play | 🟢 Pilot deployed |

**Do NOT use L0-L4 numbering.** Call them by name. Internal shorthand means nothing to investors.

**Callout box:** "We didn't raise to build the product. We built it. Now we're raising to capture the market."

---

### Section 6: Traction

**Goal:** Proof it works. Real numbers, real clients.

**Header:** "$500K ARR. $0 raised."

**Metrics bar (animated counters):**
- $500K current ARR
- $500K pipeline
- 20 people / 15 engineers
- $0 external funding

**Enterprise client grid:**
| Client | Sector | Status |
|--------|--------|--------|
| Fortune 500 Telecom | Telecommunications | 25 locations → expanding nationally |
| European Bank | Financial services | End-stage, pre-deployment |
| 5 National Debt Collection Cos | Financial services | Active, compliance-heavy |
| National Legal Services Hotline | Government | Fully deployed |

*Small text: "Enterprise clients under NDA. Industry references and metrics available upon request."*

**Case study spotlight — Debt Collection:**
- Visual: animated counter climbing to $338,357
- 0.89% abandonment rate vs 8-10% industry (show as comparison bar)
- "10x better than human call centers"
- Secure payment processing, real-time CRM updates
- 3-month implementation

**Case study 2 — Government Legal Hotline:**
- 100% call coverage, zero missed calls
- 10+ concurrent calls
- 4-month implementation
- Before/after: missing 100 calls/day → missing zero

**Design:** This section should feel like an evidence wall. Dense but clean. Numbers large, descriptions small.

---

### Section 7: The Moat

**Goal:** Why competitors can't replicate this easily.

**Header:** "Four structural advantages"

**1. Telephony exclusivity** *(not "operational lock-in")*
"You can A/B test email tools. You can run parallel chatbots. You cannot run two AI receptionists on the same phone number. One number, one system. Winner-take-all at the endpoint — by physics, not by contract."

At 50 endpoints: painful to switch. At 500: effectively permanent.

**2. Regulated industry beachhead**
Government, financial services, European banking — deployed and running. Competitors start with restaurants and spas. We started at the top. A Verizon reference sells dentists. A dentist reference doesn't sell Verizon.

**3. Five-minute deployment**
URL → live agent in 5 minutes. No other platform auto-configures a voice AI agent from a business website. GHL requires manual setup per client. This is structural — marketing automation has no single deployment artifact. Voice AI does.

**4. AEO (first-mover window)**
"When someone asks ChatGPT 'what's the best AI receptionist,' Trillet appears organically. Zero ad spend." An agency signed up after spending 1 hour interrogating ChatGPT — recommendation: "Trillet — and it wasn't even close."

**Design:** Four cards or panels, each with a bold header and one paragraph. Not a comparison table — these are unique advantages, not feature vs. feature.

---

### Section 8: Business Model

**Goal:** Show the math works. Dual revenue, high margins, compounding.

**Header:** "Two revenue streams. Both compound."

**Stream 1 — Subscriptions:**
Base monthly fee per tier. For Agency/Lite SaaS/Pro SaaS: no included minutes = nearly 100% margin on subscription.

**Stream 2 — Usage:**
Per-minute charges at 62-77% gross margin. Every call an agency's client receives generates revenue for Trillet automatically.

**The compounding visual:**
Show one agency at $299/mo → adds 10 clients → each client gets 200 calls/mo at 2 min → 4,000 min × $0.12 = $480/mo in usage alone.
Total: $299 (sub) + $480 (usage) = **$779/mo from one $299 account.**

"As agencies grow, per-minute revenue compounds without additional sales."

**Comparable raises (for context):**
Small grid:
- Retell: $5.1M seed
- Synthflow: $20M Series A
- Vapi: $20M Series A ($130M val)
- Bland: $40M Series B
- **Trillet: $500K ARR, $0 raised, product complete**

**Design:** Clean split — subscriptions on left, usage on right (or stacked on mobile). The compounding example should be an animated build-up diagram. Comparables are a simple row to anchor the ask.

---

### Section 9: Where This Goes (The Vision)

**Goal:** Show the 12-24 month trajectory AND the big picture. This is where the visionary patterns live.

**Header:** "From platform to infrastructure"

**Two timelines side by side (or stacked on mobile):**

**Now → 12 months:**
- Agency-first GTM at full velocity
- 300+ agencies on platform
- Template marketplace opens: agencies list battle-tested templates for other agencies to license
- Community and certification program launches

**12 → 24 months:**
- API Distribution powers enterprise network deployments
- The platform that agencies use becomes the infrastructure that industries run on
- Voice AI as a platform layer embedded in healthcare networks, financial systems, telecom operations

**The big frame (Pattern 10 — Factory of Factories):**
> "Bland, Vapi, and Retell built voice AI tools. GoHighLevel built a factory for marketing tools. We built the factory for voice AI tools — and our factory creates factories. Every agency on Trillet isn't just deploying voice AI. They're becoming a voice AI SaaS company."

**Two sentences to close the vision:**
> "Trillet is the platform agencies use to build, brand, and sell AI voice agents — and the infrastructure networks use to deploy them at scale."
>
> "The first sentence sells today. The second sentence sells in 12 months. Both are the same product."

**Design:** The timeline is clean two-column. The "factory of factories" quote is large, centered, on its own visual plane. The closing two-liner is the emotional peak — make it feel like a thesis statement in a darkened callout box.

---

### Section 10: The Ask

**Goal:** Clear, simple, confident close.

**Header:** "Raising $5–7M to capture the category"

**Content:**
- **Stage:** Seed+ / Pre-A
- **Use of funds:** GTM, not engineering. (15 engineers. Product is built.)
  - US sales team and agency recruitment
  - Agency community (Skool → certification → referrals)
  - Marketing and partnerships
  - Agency success team (onboarding, enablement)
  - Infrastructure scaling

**Milestone:** $500K ARR → $3-5M ARR. A few dozen → 300+ agencies. 18 months. Category leadership established before competitors realize the category exists.

**Closing line (big, centered):**
> "We built the full product stack with 20 people and $0 raised. We're at $500K ARR with a Fortune 500 expanding nationally. The agency flywheel just started turning. We're raising to capture a category that doesn't have a leader yet."

**CTA:** "Contact Ori Vaisbort — oriv@trillet.ai"

**Design:** Clean, minimal section. The pitch sentence is the visual anchor. Contact info is clear. Optional: subtle Trillet logo watermark.

---

## What NOT to Do

| Don't | Why | Instead |
|-------|-----|---------|
| Use "lock-in" | Sounds customer-hostile | "Telephony exclusivity" — structural, not strategic |
| Use "fractal" or "atomic unit" | Internal jargon | "One product, every scale" / "the core agent" |
| Use L0-L4 numbering | Meaningless to investors | Use layer names: Core AI → Agent Builder → etc. |
| Use "AEO" without explaining it | Trillet-invented term | "When you ask ChatGPT for the best AI receptionist..." |
| Claim TAM beyond voice AI | TAM inflation — VCs tune out | Stick with $6.8B → $32.6B Voice AI |
| Mix vision with traction | Undermines credibility | Traction sections = proven. Vision section = clearly future. |
| Use "white-label" unexplained | Not all investors know this | "Agencies sell Trillet under their own brand. Their clients never see our name." |
| Use "rebilling" | Not standard terminology | "Agencies bill their clients directly through our platform" |
| Show "Internal Document" banner | Wrong frame for investors | "Confidential Investor Briefing" |

---

## Source Files

All data referenced above lives in:
- [`docs/company/team.md`](../company/team.md) — full team profiles
- [`docs/company/traction.md`](../company/traction.md) — metrics, case studies, proof points
- [`docs/company/business_model.md`](../company/business_model.md) — pricing, unit economics, the ask
- [`docs/vc/market_research.md`](market_research.md) — TAM/SAM, GHL reference, competitors
- [`docs/vc/strategic_patterns.md`](strategic_patterns.md) — 10 strategic patterns to weave into narrative
- [`architecture.html`](../../architecture.html) — source for fractal visualization (adapt, don't copy)
- [`styles.css`](../../styles.css) — existing design tokens (reference for brand colors/fonts)

---

## Quality Bar

The finished artifact should feel like receiving a confidential document from a company you immediately want to fund. Not a landing page. Not a pitch deck. A narrative that builds conviction through evidence, architecture, and vision — in that order.
