# Mufasa Brand Identity — Step-by-Step Process

This document is your roadmap. We'll work through each phase in order, producing deliverables at every step. By the end, you'll have a complete brand identity usable for your website, product UI, and pitch deck.

---

## Phase Overview

```
Phase 1: Brand Strategy        → The foundation. Everything flows from here.
Phase 2: Naming & Voice        → What we say and how we say it.
Phase 3: Visual Identity       → Logo, colors, typography, imagery.
Phase 4: Design System         → CSS tokens + component library.
Phase 5: Brand Guidelines      → The compiled, shareable rulebook.
Phase 6: Applications          → Pitch deck, website, product UI mockups.
```

---

## Phase 1: Brand Strategy
**Goal:** Define who Mufasa is, for whom, and why it matters — before touching any visuals.

### Step 1.1 — Positioning Statement
We'll write a single, precise positioning statement that anchors all future decisions:
> *"For [segment] who [pain], Mufasa is the [category] that [benefit], unlike [alternative] which [limitation]."*

**Session prompt:** *"Let's write the Mufasa positioning statement. Ask me the questions you need."*

### Step 1.2 — Brand Archetype
We'll select 1 dominant + 1 supporting archetype from the 12 brand archetypes. This determines personality, visual direction, and tone.

**Most likely candidates for Mufasa:**
- **The Ruler** — commands authority, built for professionals, premium
- **The Magician** — transforms how things work (6hrs → 30min)
- **The Sage** — deep expertise in a complex domain

**Session prompt:** *"Let's choose the Mufasa brand archetype."*

### Step 1.3 — Brand Pillars
3–4 core values that every brand decision must serve.

**Session prompt:** *"Let's define the Mufasa brand pillars."*

### Step 1.4 — Competitive Positioning Map
Where Mufasa sits vs. Wetu, SafariPortal, Waybird, Tourplan — visually expressed as a 2×2 or positioning diagram. Useful for pitch deck slides too.

**Already pre-loaded:** Full competitor context is in CLAUDE.md.

---

## Phase 2: Naming & Voice
**Goal:** Define what we call things and how the brand speaks.

### Step 2.1 — Tagline Development
Generate and evaluate 10–15 tagline options across different strategic directions (functional, emotional, aspirational). Select and refine to 1 hero tagline + 2 alternates.

**Session prompt:** *"Let's develop tagline options for Mufasa."*

### Step 2.2 — Tone of Voice
Define how Mufasa sounds across: website hero copy, in-app microcopy, sales emails, error messages, social, pitch deck. Produce a tone guide with examples.

**Session prompt:** *"Let's define the Mufasa tone of voice."*

### Step 2.3 — Nomenclature
What do we call: the product's modules, the user types, actions, pricing tiers?

---

## Phase 3: Visual Identity
**Goal:** The logo, color system, and typography that make Mufasa instantly recognisable.

### Step 3.1 — Moodboard & Direction
Before pixels, align on the visual world. We'll define 2–3 distinct visual directions and choose one.

**Direction candidates to explore:**
- **Dark & Confident:** Deep midnight + gold. Think Linear, Stripe. Premium, authoritative.
- **Earthy & Modern:** Warm terracotta, clay, warm whites. Africa-rooted but tech-forward.
- **Clean & Expansive:** White space, savannah ochre accent, crisp black. Editorial luxury.

**Session prompt:** *"Let's explore visual directions for Mufasa."*

### Step 3.2 — Color System
Primary, secondary, tertiary, neutrals, semantic colors. Define every hex value with rationale. Update `mufasa-style-guide.css`.

**Session prompt:** *"Let's define the Mufasa color palette."*

### Step 3.3 — Typography System
Select display, heading, and body fonts. Define size scale, weight usage, and line-height rules.

**Session prompt:** *"Let's choose the Mufasa type system."*

### Step 3.4 — Logo Concepts
Describe the logo direction and generate visual concepts. Evaluate and refine.

**Session prompt:** *"Let's develop logo concepts for Mufasa."*

### Step 3.5 — Imagery & Photography Direction
Define the visual language for photography: subjects, mood, color treatment, what to avoid.

---

## Phase 4: Design System
**Goal:** A practical CSS system and component library that anyone can implement.

### Step 4.1 — CSS Design System
Update `visual-identity/mufasa-style-guide.css` with all final token values.

### Step 4.2 — Component Library (HTML)
Build key UI components as HTML/CSS:
- Buttons (primary, secondary, ghost, destructive)
- Form inputs
- Cards
- Navigation / sidebar
- Data tables
- Proposal preview card
- Badge / tag component
- Modals

**Session prompt:** *"Build the Mufasa UI component library."*

### Step 4.3 — Key Screen Mockups
Full-page HTML mockups of:
1. Agent dashboard (home)
2. Itinerary builder view
3. Digital proposal (client-facing)
4. Pricing / subscription page

---

## Phase 5: Brand Guidelines
**Goal:** A single compiled document — the brand bible.

### Step 5.1 — Compile BRAND_GUIDELINES.md
A complete, structured brand guidelines document covering all phases above. Shareable with designers, developers, marketing partners, and investors.

**Sections:**
1. Brand Story
2. Mission & Vision
3. Brand Personality & Archetype
4. Brand Pillars
5. Tagline & Messaging
6. Tone of Voice
7. Logo System
8. Color Palette
9. Typography
10. Iconography
11. Photography Direction
12. UI Design Principles
13. Applications
14. What to avoid (brand donts)

---

## Phase 6: Applications
**Goal:** Proof-of-concept applications of the brand for pitch and web.

### Step 6.1 — Pitch Deck Brand Application
Apply the brand to key pitch slide designs. Produce as HTML/CSS mockups or CSS style guide for the existing PowerPoint.

### Step 6.2 — Website Hero Section
Build a premium HTML/CSS landing page hero section using the finalized brand.

### Step 6.3 — Email Signature & Social Assets
Define templates for team email signatures and social media profile assets.

---

## How to Start Each Session

Just tell Claude which step you want to work on. For example:
- *"Let's start Phase 1, Step 1.1 — positioning statement."*
- *"I want to explore color palettes today — let's do Phase 3, Step 3.2."*
- *"Generate 3 visual design directions for Phase 3.1."*

Claude will guide you with questions, generate options, and produce files into the appropriate folders.

---

## Deliverables Tracker

| Deliverable | Phase | Status |
|---|---|---|
| Positioning statement | 1.1 | 🔲 |
| Brand archetype | 1.2 | 🔲 |
| Brand pillars | 1.3 | 🔲 |
| Tagline (hero + 2 alts) | 2.1 | 🔲 |
| Tone of voice guide | 2.2 | 🔲 |
| Color system | 3.2 | 🔲 |
| Typography system | 3.3 | 🔲 |
| Logo concepts | 3.4 | 🔲 |
| mufasa-style-guide.css (final) | 4.1 | 🔲 |
| UI component library | 4.2 | 🔲 |
| Agent dashboard mockup | 4.3 | 🔲 |
| Client proposal mockup | 4.3 | 🔲 |
| BRAND_GUIDELINES.md | 5.1 | 🔲 |
| Pitch deck brand application | 6.1 | 🔲 |
| Website hero section | 6.2 | 🔲 |
