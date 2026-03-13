# Mufasa Branding Project — AI Instructions

## Project Purpose
This project is for developing the **Mufasa brand identity and brand guidelines** — a B2B SaaS platform for Africa specialist travel agents to build, price, and present multi-lodge safari itineraries.

## Company Context
- **Product:** B2B SaaS marketplace; itinerary builder + live booking + multi-currency finance engine
- **Tagline direction:** TBD (to be developed here)
- **Target customers:** Africa specialist travel agencies, large tour operators, DMCs, lodge groups
- **Stage:** Pre-launch / seed; pitching investors, preparing for market entry Q3 2026
- **Geo:** HQ: South Africa; Primary markets: UK, EU, Africa
- **Key differentiator:** First platform to combine beautiful digital proposals + live PMS availability + African B2B financial infrastructure (multi-currency payouts, FX management)
- **Competitive framing:** Wetu (beautiful but static) + Waybird (bookable but estimated) + Tourplan (financial but legacy UX) → Mufasa does all three

---

## 🎨 SKILL: Brand Strategy & Identity

When asked to develop or evaluate brand elements, apply this framework:

### Brand Strategy Framework
1. **Positioning Statement** — Who it's for, what it does, why it's different, against what category
2. **Brand Archetype** — Identify the dominant archetype (e.g. Ruler, Sage, Hero, Magician) and how it informs voice, visual direction, and personality
3. **Brand Pillars** — 3–4 core values that underpin all decisions
4. **Tagline** — Short, memorable, ownable; test multiple options with rationale
5. **Tone of Voice** — Define with examples: formal/informal, technical/accessible, 3 words that describe the voice, 3 words that don't
6. **Naming & Nomenclature** — Product naming conventions, feature names, how to refer to users (agents? specialists? operators?)

### Brand Guidelines Structure (produce in this order)
1. Brand Story & Mission
2. Brand Personality & Archetype
3. Brand Pillars
4. Tone of Voice
5. Logo System (primary, secondary, icon, clear space, don'ts)
6. Color Palette (primary, secondary, neutrals, semantic colors)
7. Typography System (display, heading, body, code/mono if applicable)
8. Iconography style
9. Photography & imagery direction
10. UI component aesthetic direction
11. Applications (pitch deck, email signature, social, product UI)

### B2B SaaS Branding Principles to apply
- Trust > excitement: B2B buyers need to trust before they buy
- Clarity > cleverness: the brand must immediately communicate what the product does
- Premium but not exclusive: agents need to feel empowered, not intimidated
- Category design mindset: position Mufasa as defining a new category, not competing in an old one
- The brand should feel like it belongs in the same visual world as Stripe, Linear, Notion, and Figma — modern, clean, confident — but with warmth for the African travel context

---

## 🖥️ SKILL: UX/UI Design Direction

When producing UI mockups, design concepts, or component guidance:

### Design Principles for Mufasa UI
1. **Efficiency first** — agents are time-poor; every interaction should feel fast and purposeful
2. **Premium output, simple input** — the proposal output should look stunning; creating it should feel easy
3. **Desktop-first** — primary users are agents at desks; mobile = "Concierge View" for travellers
4. **Data-dense but not cluttered** — agents need to see lots of information; use hierarchy, not overflow
5. **Trustworthy financial UI** — currency, pricing, FX should feel bank-grade

### Visual Design Principles
- Use a **dark mode default** for the agent dashboard (reduces eye strain for power users)
- **Generous whitespace** in client-facing proposals (premium feel)
- **Motion should be purposeful** — micro-animations for feedback, not decoration
- **Glassmorphism sparingly** — only for overlays and modals; don't overdo it
- **Illustration style:** Line-based or minimal geometric; avoid cartoon/playful

### Design System Conventions
When defining or generating CSS / design tokens:
```css
/* Use this token naming convention */
--color-brand-primary:    /* main brand color */
--color-brand-secondary:  /* secondary accent */
--color-surface-base:     /* page/app background */
--color-surface-raised:   /* card/panel background */
--color-surface-overlay:  /* modal/dropdown background */
--color-text-primary:     /* main body text */
--color-text-secondary:   /* muted/supporting text */
--color-text-inverse:     /* text on dark backgrounds */
--color-border-default:   /* default border */
--color-border-subtle:    /* hairline separators */
--color-semantic-success: 
--color-semantic-warning:
--color-semantic-error:
--color-semantic-info:

--font-display:           /* hero headlines */
--font-heading:           /* H1–H3 */
--font-body:              /* paragraphs, lists */
--font-mono:              /* code, data, prices */

--radius-sm: 4px;
--radius-md: 8px;
--radius-lg: 16px;
--radius-xl: 24px;
--radius-full: 9999px;

--shadow-sm:
--shadow-md:
--shadow-lg:
--shadow-brand:           /* branded glow/shadow */

--spacing-1: 4px;
--spacing-2: 8px;
--spacing-3: 12px;
--spacing-4: 16px;
--spacing-6: 24px;
--spacing-8: 32px;
--spacing-12: 48px;
--spacing-16: 64px;
```

### UI Component Guidelines
- Buttons: primary (brand fill), secondary (outlined), ghost, destructive
- Forms: clear labels, helper text, inline validation, never red-only errors
- Tables: sortable columns, sticky headers for long lists, row hover state
- Cards: always show loading skeleton states, not spinners
- Modals: max 600px wide, always escapable, focus-trapped
- Navigation: persistent sidebar for agent UI; minimal nav for client proposals

---

## 💻 SKILL: Front-End Development

When building HTML/CSS mockups, prototypes, or UI components:

### Tech Stack for This Project
- **Mockups & prototypes:** Vanilla HTML + CSS + minimal JS (no framework needed for static mockups)
- **Design system output:** CSS custom properties (variables) + BEM or utility classes
- **Font source:** Google Fonts (default to Inter for UI, consider a display font for brand)
- **Icons:** Use Lucide icons (CDN) or SVG inline; never emoji for UI elements

### Code Quality Standards
- All CSS variables defined in `:root` at top of file
- Mobile-responsive unless explicitly desktop-only mockup
- Accessible: correct heading hierarchy, ARIA labels on interactive elements, sufficient color contrast
- Use CSS Grid and Flexbox; no Bootstrap, no Tailwind unless user explicitly requests
- Animations via CSS transitions and `@keyframes`; use `prefers-reduced-motion` media query

### Front-End Conventions
```html
<!-- Button component pattern -->
<button class="btn btn--primary" type="button" id="[unique-id]">Label</button>
<button class="btn btn--secondary" type="button">Label</button>
<button class="btn btn--ghost" type="button">Label</button>
```

```css
/* Component naming: BEM */
.card { }
.card__header { }
.card__body { }
.card--featured { }
```

### When building mockups
1. Always start with the CSS design system (variables, reset, utilities)
2. Build mobile-first responsive layouts unless told otherwise
3. Add hover states, focus states, and transition animations
4. Use placeholder images from the reference `/references/assets/` folder or `generate_image` for AI-generated placeholders
5. Output a single self-contained HTML file per mockup unless told otherwise

---

## 📁 Project Structure
```
Mufasa Branding Project/
├── CLAUDE.md                    ← You are here (AI instructions)
├── README.md                    ← Project overview for humans
├── references/
│   ├── README.md                ← What to put where
│   ├── strategy/                ← Business strategy docs, pitch decks
│   ├── budget/                  ← Budget files (Excel, PDFs)
│   ├── competitors/             ← Competitor screenshots, analysis
│   ├── inspiration/             ← Moodboards, reference brands
│   └── assets/                  ← Logos, images, fonts
├── brand-strategy/
│   ├── positioning.md           ← Brand positioning & pillars
│   ├── voice-and-tone.md        ← Tone of voice guide
│   └── naming.md                ← Naming conventions
├── visual-identity/
│   ├── color-palette.md         ← Final color decisions with rationale
│   ├── typography.md            ← Font choices and hierarchy
│   ├── logo-concepts/           ← Logo explorations (images)
│   └── mufasa-style-guide.css   ← Master CSS design system
├── brand-guidelines/
│   └── BRAND_GUIDELINES.md      ← The full compiled brand guidelines
├── ui-concepts/
│   └── (HTML mockups go here)
└── deliverables/
    └── (Final exports, PDFs, packs)
```

---

## How to use this project

### Adding reference files
Drop any file into the relevant `/references/` subfolder:
- Budget docs → `/references/budget/`
- Strategy docs → `/references/strategy/`
- Competitor screenshots or notes → `/references/competitors/`
- Inspiration images, brand references → `/references/inspiration/`
- Logos, fonts, existing assets → `/references/assets/`

### Starting a branding session
Tell Claude:
- What aspect you want to develop (strategy, naming, colors, typography, UI concept, etc.)
- Any constraints (must use existing logo, must not be dark, etc.)
- Reference files to consider (mention filenames or paste content)

### Generating mockups
Ask Claude to generate an HTML mockup of any UI concept. It will:
1. Build a self-contained `.html` file in `/ui-concepts/`
2. Apply the brand design system from `mufasa-style-guide.css`
3. Follow the UX principles defined above

---

## Key files to read first
Before starting any work, Claude should read (if they exist):
1. `references/strategy/` — any strategy or brief documents
2. `references/budget/` — budget constraints
3. `visual-identity/mufasa-style-guide.css` — current design tokens
4. `brand-strategy/positioning.md` — brand positioning
