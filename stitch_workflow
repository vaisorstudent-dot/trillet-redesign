Run a Stitch-first workflow that prevents “mid-tier vibe coding” by locking decisions early, generating a strong design scaffold, then using Stitch MCP + Stitch Agent Skills to build and iterate with a QA loop.

## Workflow overview
The system is: Decide → Research → Blueprint → Design (Stitch) → Build + Validate. The key rule is that every unanswered question in your plan becomes a forced guess by the model at build time, so you front-load decisions.

## Step 0: Decide (pre-flight upgrades)
Write a one-page decision log before you touch Stitch or code:
- Audience: who exactly (job, sophistication, context).
- Primary CTA: one verb (book, start, download, install).
- Promise: one sentence outcome; 3 supporting benefits.
- Proof inventory: 3 assets you can show now (numbers, screenshots, testimonials, logos, demos).
- Objections: 5 bullets you must answer (price, time, trust, setup, “will it work for me?”).
- Constraints: brand vibe (3 adjectives), must-have sections, must-not-do (no gradients, no illustrations, etc.).

This single doc prevents “design drift,” makes later iterations faster, and gives you a stable target for A/B testing.

## Step 1: Research (direct + indirect)
Use your competitive landscape prompt (direct and indirect competitors) and extract two things you’ll reuse verbatim:
- Messaging primitives: common pains, promises, differentiation patterns, proof types, and tone.
- Structure primitives: which sections appear, in what order, and what each section *does* (not just what it’s called).

Prompt (template):
```
Competitive Landscape Analysis

Context
I run [business/product]. My target audience is [persona]. I offer [offer].

Objective
Conduct a comprehensive competitive analysis of both direct and indirect competitors to
inform strategic positioning and identify market opportunities.

Research Scope
Direct Competitors
Find 5–8 companies/creators who:
Serve the same target audience
Offer similar solutions/products
Compete for the same buyer intent

Indirect Competitors
Find 3–5 companies/creators who:
Solve the same problem differently
Target adjacent audiences with transferable solutions
Represent alternative approaches to the same outcome

Analysis Framework
For each competitor, analyze:
Primary value proposition (hero)
Target audience positioning
Problem/solution framing
Differentiation claims
Brand identity cues
Landing page structure (sections + flow)
```

## Step 2: Blueprint (3 hypotheses + page copy)
Force multiple positioning drafts so you don’t lock in too early, then pick one to implement first and keep the others as test variants.

Prompt (template):
```
Using the competitive analysis above, create a landing page blueprint.

Requirements:
- Produce 3 competing positioning hypotheses:
  1) Efficiency + scale
  2) Quality + nuance
  3) Personalization + applying the customer’s frameworks
- For each hypothesis, provide:
  - Hero: headline, subheadline, primary CTA, secondary CTA
  - Proof plan: what evidence to show in what format
  - 3–6 feature→benefit sections
  - How it works (3 steps)
  - Pricing structure (tiers + what belongs)
  - FAQs (6–10) aimed at objections
Constraints:
- Use competitor language patterns, but don’t copy phrases.
- Be concrete; ban generic SaaS filler.
```

Upgrade: output your hero in 2–3 variants *per hypothesis* (so you can test without redesigning).

## Step 3: Design in Google Stitch (scaffold → inject copy)
The highest-leverage pattern is to generate **scaffolding** first (layout + style system), then paste in your finalized copy to keep strong hierarchy.

Prompts (templates):
```
(Scaffold)
Design a modern landing page for [offer] targeting [persona].
Use placeholder copy. Prioritize hierarchy, spacing, typography, and consistent components.
Sections: hero, proof, benefits, how-it-works, pricing, FAQ, final CTA.

(Inject copy)
Keep the exact same layout and styling.
Replace placeholder text with this copy, section by section:
[PASTE FINAL COPY]
```

Optional upgrades to explore distinct “design DNA” quickly:
- Add a named style constraint (e.g., claymorphism).
- Use a reference image as style inspiration, then iterate with “tone it down / more premium / less techy / more playful.”

## Step 4: Build + validate loop (MCP + skills + QA)
Connect your IDE to Stitch via Stitch MCP (follow the Stitch MCP setup docs for your environment).  Use Stitch Agent Skills so the agent can extract a design system into a `DESIGN.md` (“design-md”) and generate React components (“react-components”) that match the Stitch design. [stitch.withgoogle](https://stitch.withgoogle.com/docs/mcp/setup)

Publicly shown install commands:
```
npx add-skill google-labs-code/stitch-skills --skill design-md
npx add-skill google-labs-code/stitch-skills --skill react-components
``` 


Build prompt (template):
```
Use the Stitch MCP connection and the installed Stitch skills in this repo.
Build the Stitch design named “[DESIGN_NAME]” into working code.
Match layout, spacing, typography, colors, and components.
Use DESIGN.md as the source of truth; do not invent new styles.
```

Validation upgrades (this is where “good-looking” becomes production-ready):
- Accessibility pass: labels, focus states, contrast, keyboard nav.
- Performance pass: image sizes, lazy loading, LCP/CLS budget.
- Visual regression: screenshot key breakpoints; re-run after edits.
- Architecture hygiene: keep copy in one data file, keep components small, isolate behavior in hooks, and don’t let generated code sprawl.

Experiment upgrade: ship 2–3 hero variants behind a query param and track CTA clicks → downstream conversion so you pick winners by data, not taste.