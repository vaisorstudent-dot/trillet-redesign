# Trillet — Decisions Needed Before Deck Goes Out

**From:** SaaS Advisory Panel Assessment (Feb 28, 2026)
**To:** Ming, Laurence, Ori
**Action required by:** Before investor deck is sent

---

## Context

We ran a 5-agent SaaS consulting simulation against investor_v3.html and all supporting docs. Full assessment is in `docs/vc/saas_assessment.md`. This is the one-pager: 6 decisions, each with the tradeoff and a recommended path.

---

## Decision 1: Which business are we pitching?

**The problem:** 65% of our $500K ARR is enterprise (Verizon, debt collection, legal hotline). 10% is agency (~14 paying accounts). The deck says "agency-first." Investors will see the mismatch immediately.

**Options:**
- **(A) Lead with enterprise, position agency as scale mechanism.** "We proved the product with Fortune 500s. Enterprise validates quality. Agency distributes it." Phased GTM: months 0-9 enterprise-led/agency-seeded, months 9-18 agency-scaled if metrics hit.
- **(B) Keep agency-first framing.** Double down on GHL narrative. Accept that the evidence gap is the raise's weakness and address it head-on.

**Recommendation:** A. It's honest, leverages our strongest asset, and buys time to generate agency evidence.

**Who decides:** All three founders. This changes the entire deck narrative.

---

## Decision 2: D2C channel conflict — what's our position?

**The problem:** We sell D2C at $59/mo. We recruit agencies to resell at $200-500/mo markup. If AEO works (and we claim it does), SMBs find us directly and have zero reason to pay an agency 4-8x. GHL never had this problem because they don't sell to end-SMBs.

**Options:**
- **(A) Make trillet.ai agency-facing.** D2C becomes "get started yourself or find a Trillet agency partner" with a partner directory. Protects agency economics.
- **(B) Feature-gate D2C.** $59 gets basic agent. Agencies unlock premium features (multi-agent, CRM sync, advanced integrations). Creates real agency value-add.
- **(C) Accept cannibalization.** "Some SMBs self-serve, some want managed. Market sorts itself." Requires a compelling explanation for why agencies still win.
- **(D) Geographic/vertical segmentation.** Agencies get territories. Complex at scale.

**Recommendation:** B. Preserves AEO advantage, gives agencies defensible value-add, doesn't require killing a revenue stream.

**Who decides:** Ori + Ming. This affects product roadmap (what gets gated) and site architecture.

---

## Decision 3: Cap Agency tier at 20 sub-accounts?

**The problem:** Agency at $299/mo gives unlimited agents + white-label + rebilling. At 20 clients, that's $14.95/client — leaving 5-10x on the table. Lite SaaS at $497 adds templates and self-onboarding (convenience), but Agency already has rebilling (revenue). No rational buyer upgrades. Lite SaaS is a dead tier.

**The fix:** Cap Agency at 20 sub-accounts. Lite SaaS ($497) becomes "scale past 20 clients." Graduation trigger aligns with agency success (they only hit the cap if their business is working).

**Revenue impact:** At 100 agencies, a 20-client cap adds ~$143K/yr in incremental subscription revenue (31% increase).

**Risk:** Some early agencies may push back. But we have ~14 paying accounts — most likely have <20 clients. The window to introduce this is NOW, before expectations calcify.

**Options:**
- **(A) Implement 20-client cap before GTM push.** Ship it, update pricing page, reframe Lite SaaS.
- **(B) Keep unlimited, revisit at 100 agencies.** Preserves simplicity but locks in underpricing.
- **(C) Test with new signups only.** Grandfather existing agencies at unlimited, cap new ones.

**Recommendation:** A (or C if existing agencies are a concern). Do this before the round closes.

**Who decides:** Ori + Ming. Ming implements, Ori owns pricing narrative.

---

## Decision 4: How do we answer "why isn't Ming the CEO?"

**The problem:** The deck's origin story is titled "He didn't predict the category. He lived the gap" — about Ming. Ming built L0-L4. Ming is the founder-market-fit story (Bland.ai's first partner, 7-figure exit). Ming is titled COO. Laurence is CEO with a healthcare SaaS background. Every investor will ask this.

**This is not a suggestion to change titles.** It is a requirement that all three of you deliver the same crisp answer without hesitation.

**Draft answer (adapt as needed):** "Ming builds the product and leads technical strategy. Laurence runs the company — operations, compliance, enterprise delivery. Ori opens the US market. We split by function, not hierarchy. Ming doesn't want to be CEO — he wants to build."

**Who decides:** All three founders. Write the answer, rehearse it, deliver it identically.

---

## Decision 5: Raise $5M or $7M?

**The problem:** Post-raise burn is $2.5-3.3M/yr. At $5M, pessimistic runway is 10-12 months — not enough for a second chance if the agency motion takes longer than expected. At $7M, pessimistic runway is 14-16 months.

**The math:**

| Raise | Optimistic Runway | Pessimistic Runway | Room to Pivot? |
|-------|------------------|--------------------|----------------|
| $5M | 16-18 months | 10-12 months | No |
| $7M | 20-24 months | 14-16 months | Yes |

**Recommendation:** Target $7M. The extra dilution is worth the optionality. The difference between $5M and $7M is the difference between one shot and two.

**Who decides:** Ori (fundraising lead), with input from all founders on dilution tolerance.

---

## Decision 6: First US hire — who and when?

**The problem:** 90% of the raise goes to US GTM. Ori is the only US person. He's doing enterprise sales + agency GTM + fundraising + will manage new hires. That's 3-4 jobs.

**Recommended first hire:** Head of Agency Sales. IC who can close AND build the playbook. Not a VP who manages a team that doesn't exist. $220-250K fully loaded. Start sourcing NOW, target offer within 60 days of close.

**Sequencing (all 5):**

| Order | Role | Timing | Cost |
|-------|------|--------|------|
| 1 | Head of Agency Sales (US) | Month 1-2 | $220-250K |
| 2 | Solutions Engineer (US West Coast) | Month 2-3 | $180-200K |
| 3 | Agency Success Manager | Month 4-5 | $130-160K |
| 4 | Agency SDR/BDR | Month 5-6 | $90-120K |
| 5 | Community & Content Lead | Month 5-7 | $110-140K |

**Who decides:** Ori drafts the JD for #1 and #2. Ming validates technical requirements for #2 (Solutions Engineer needs AU-hours flexibility). Begin sourcing before the round closes.

---

## One More Thing: The Agency Case Study

This isn't a decision — it's a blocker. Every analysis we ran (VC panel, SaaS panel) converges on the same point: **zero agency evidence kills the raise.**

Ori: pick the best-performing of the ~14 paying agencies. Get permission. Document: how many clients they've deployed, usage revenue, time from onboarding to first deployment, what they charge their clients. Even n=1 changes the conversation from "will agencies use this?" to "here's what it looks like."

**Timeline:** This week. Before the deck goes to anyone.

---

*Full assessment with competitive analysis, pricing deep-dive, org scaling model, and 90-day roadmap: `docs/vc/saas_consulting_assessment.md`*
