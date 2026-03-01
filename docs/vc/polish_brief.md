# Investor Artifact — Polish Brief (V2)

*For: Builder agent (polish pass)*
*Input: `investor.html` (existing, 2343 lines)*
*Goal: Elevate visual execution from "clean developer site" to "confidential document from a company you want to fund"*

**CRITICAL: Do NOT change the narrative content, section order, or data. The content is correct. This is purely a visual/interaction polish pass.**

---

## Issue 1: Hook Section Has Too Little Visual Weight

**Problem:** The hero is a full viewport of dark with small centered text. It feels empty, not dramatic.

**Fix:**
- Increase hook text size — the first line ("A Fortune 500 telecom...") should be `clamp(1.375rem, 3vw, 1.875rem)` at minimum
- Add a subtle animated background element — a soft radial pulse or slowly drifting gradient orbs behind the text (very subtle, 3-5% opacity)
- The "$338,000" and "0.89%" numbers should be noticeably larger than surrounding text — make them feel like data callouts, not inline text
- Add a subtle downward scroll indicator (small animated chevron or "scroll" text) at the bottom of the viewport

---

## Issue 2: Brand Reveal Section Is Dead Weight

**Problem:** The "Trillet AI / CONFIDENTIAL INVESTOR BRIEFING" interstitial between hook and market section looks like a blank title slide.

**Fix — two options (pick one):**
- **Option A:** Remove it entirely. The confidential bar at top already brands. Let the flow go straight from hook → market.
- **Option B:** Make it minimal — just a thin horizontal rule with the Trillet dot logo centered, acting as a visual breath between hook and content. No large text.

**Recommendation:** Option A.

---

## Issue 3: Every Section Looks Identical — No Visual Rhythm

**Problem:** Cards → text → cards → text. No section feels different from any other. The traction section should feel like an evidence wall. The vision section should feel aspirational. The moat section should feel defensive/solid.

**Fixes by section:**

### Market Section (The Gap)
- The $6.8B → $32.6B numbers are good but need a visual connector — add a thin animated line or gradient bar between them suggesting growth trajectory
- The competitor cards should have a subtle red/warning tint to distinguish them from Trillet's teal. They represent "wrong approach" — make that visual.

### Traction Section
- This should be the DENSEST section — the evidence wall. Tighten spacing. Make the metrics bar numbers LARGE and impactful.
- The $338,357 counter should be the hero moment — give it extra size (`clamp(2.5rem, 5vw, 3.5rem)`), maybe a subtle teal glow or text-shadow
- The comparison bars (Trillet 0.89% vs Industry 8-10%) are great — add a "~10x better" label that appears after the bars animate, in bold teal

### Moat Section
- Give each moat card a distinct left-border color instead of all using the same card style:
  - Telephony exclusivity: teal border
  - Regulated beachhead: amber border
  - 5-min deployment: blue border
  - AI-native discovery: indigo border
- The "kicker" lines (italicized at bottom of each card) are great — make them slightly more prominent

### Vision Section
- This should feel DIFFERENT from everything before it — it's the future, not the present
- Add a very subtle background shift — slightly different background tone for this section (e.g., a barely-visible indigo-tinted gradient)
- The factory-of-factories quote needs a premium treatment: consider a larger font size, more padding, and a subtle border gradient (teal → indigo) on all sides, not just top

---

## Issue 4: The Thesis Box and Closing Statement Need Distinction

**Problem:** The thesis ("Trillet is the platform agencies use to build, brand, and sell...") and the closing pitch sentence look like regular callout boxes. These are the two most important pieces of text on the entire page.

**Fix:**
- **Thesis box:** Increase font size to `clamp(1.125rem, 2.2vw, 1.375rem)`. Add `font-weight: 600`. The "first sentence / second sentence" line should have a different visual treatment — smaller, lighter, almost like a whispered punchline after the main statement
- **Closing statement (The Ask section):** This is the FINAL impression. Give it a subtle background animation — a very slow gradient shift or a pulsing glow around the border. The investor should feel the text resonate.

---

## Issue 5: GHL Box Needs More Impact

**Problem:** The GHL stats (2M+, 781%, $2B+) are in a plain box. These numbers are supposed to make the investor think "wow, this model works at massive scale."

**Fix:**
- Make the stat numbers larger — `clamp(2rem, 4vw, 2.75rem)` instead of current 2rem
- Add a subtle counter animation to these numbers (similar to the traction counters)
- Consider adding a thin teal → amber gradient border to the GHL box to make it feel special
- The "Voice AI has no equivalent. We're building it." line should be on its own line, larger, bolder — it's the single most important sentence in the section

---

## Issue 6: The Ask Section Needs a Stronger Close

**Problem:** The $5-7M number is big but the section feels like it tapers off.

**Fix:**
- The 5 use-of-funds cards need icons (not just colored dots). Use simple Unicode or SVG icons:
  - 🎯 US sales team
  - 👥 Agency community
  - 📢 Marketing
  - 🤝 Agency success
  - ⚡ Infrastructure
- Or use small, clean SVG circles with different fill colors to differentiate
- Add a subtle "Founded September 2024 — Melbourne, Australia" line near the contact info — grounds the company in reality
- The contact section should feel warmer — "Let's talk" instead of just "Contact"

---

## General Polish

1. **Add smooth section dividers.** Instead of just `border-bottom`, consider subtle gradient fades between sections — a thin line that fades from transparent → teal/amber → transparent.

2. **Increase contrast on key numbers.** Any metric or dollar amount should have a subtle `text-shadow: 0 0 40px rgba(color, 0.15)` to make them glow against the dark background.

3. **Active nav highlight.** As the user scrolls, highlight the corresponding section in the nav bar. Add an `active` class to the nav link when its section is in view.

4. **Add a subtle noise/grain texture** to the body background. Very light (1-2% opacity). This removes the "flat digital" feel and adds depth. Use CSS `background-image` with a small repeating pattern or SVG filter.

5. **Typography polish:** Ensure section labels (THE OPPORTUNITY, THE PRODUCT, etc.) have generous letter-spacing (`0.15em+`) and feel like elegant whispers, not shouting.

---

## What NOT to Change

- Section order
- Narrative content / copy
- Data / numbers
- Color palette (teal, amber, indigo)
- Font family (Inter)
- Mobile responsiveness approach
- Animation timing / reveal approach
- Deployment tier interactive visualization (it's working well)

---

## Quality Bar

After this polish pass, an investor should:
1. Be stopped cold by the hook (the numbers + bootstrapped claim create "tell me more" urgency)
2. Feel the traction section as an evidence WALL (dense, undeniable)
3. Experience the moat section as structural / inarguable
4. Arrive at the vision feeling like the trajectory is inevitable
5. Leave the page wanting to take a meeting

The page should feel like a Stripe or Linear marketing page — not a pitch deck rendered in HTML.
