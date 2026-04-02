# Arize Consulting - Website Design Spec

## Context

Arize Consulting is Jan Vaes' boutique AI advisory practice targeting Flemish SMEs (Limburg first, 50-500 employees, traditional sectors). The company is pre-revenue and founder-led. The website's job is to sell one thing: the AI Readiness Assessment, a facilitated diagnostic session. Jan's COO consulting background provides credibility but is not a service being sold on this site.

## Decisions Made

| Decision | Choice | Rationale |
|---|---|---|
| Page type | One-pager | Single offer, early stage, no need for multi-page |
| Language | Dutch (Flemish) | Limburg-first market, local feel |
| Core offer | AI Readiness Assessment (facilitated) | First product to validate face-to-face |
| Pricing | Not shown ("op aanvraag") | Still validating, need flexibility |
| CTA | Contact form | Relationship-driven market, Jan follows up personally |
| Positioning | Jan the person, not "a company" | Founder-led, Limburg buyers buy from people |
| Page structure | Problem-Solution flow (Approach A) | Mirrors buyer journey: fear > concrete pain > solution > trust |
| Company names | Not mentioned by name | Need permission first; use generic descriptions |
| Brand colors | Navy (#2B3044), Gold (#D4993D), White | Extracted from existing logo assets |

## Target Audience

- Flemish SMEs, 50-500 employees, primarily Limburg
- Traditional sectors: logistics, manufacturing, professional services
- Decision makers: COOs, operations managers, managing directors of family businesses
- Not tech companies, not tech-savvy audiences
- Buyer trigger: fear of falling behind on AI, then recognition of concrete operational waste

## Brand & Tone

- Direct, no-nonsense, Flemish B2B register
- Practitioner credibility: "I do this every day" not "we advise on best practices"
- No anglicisms where normal Dutch works
- No buzzwords: avoid "transformatie," "cutting-edge," "toekomstbestendig," "AI-gedreven oplossingen"
- Short sentences, scannable, every section should earn its place

## Page Structure

### 1. Navigation (sticky)

- Background becomes slightly opaque/blurred on scroll
- **Desktop (md: 768px+):** Logo (left) + scroll anchors "Over Jan" | "Contact" + CTA button "Neem contact op" (right)
- **Mobile (<768px):** Logo (left) + CTA button (right). Drop scroll anchors entirely — the page is short, the user scrolls. No hamburger menu.

### 2. Hero

**Goal:** Immediate gut-punch. Name the fear, offer a way out.

- **Headline:** Hook around "your competitors are already using AI, you're not" (exact Dutch copy TBD during implementation, direction is clear)
- **Subline:** One sentence bridging to the assessment. Direction: "Ontdek in 90 minuten waar AI u concreet tijd en geld bespaart."
- **CTA button:** "Neem contact op" — scrolls to contact form section
- **Design:** Typography-driven, no hero image. Navy or white background. Gold accent on CTA button.

### 3. Problem

**Goal:** Make the vague fear concrete with 3 recognizable pains.

- **Section title:** Something like "Herkenbaar?" or "Wat u elke dag ziet"
- **3 pain points**, each one sentence:
  1. Manual data copying between systems, every day
  2. Everyone talks about AI, nobody knows where to start
  3. Investing in tools nobody actually uses
- **Format:** Icon or number + text. Short, scannable. No paragraphs.

### 4. Assessment (The Offer)

**Goal:** Introduce the AI Readiness Assessment as the direct answer.

- **Section title:** Direction: "De AI Readiness Assessment" or "Weet waar te beginnen"
- **Intro:** 2 sentences max. What it is, who it's for.
- **Deliverables list:**
  - 3-5 concrete AI-kansen, gerankt op impact en haalbaarheid
  - 1 quick win uitvoerbaar binnen 30 dagen
  - 1 waarschuwing specifiek voor hun situatie
  - Een helder actieplan, geen vaag rapport
- **Explicit framing:** This is not a maturity scan with a radar chart. It's a prioritized action list tied to their business.

### 5. How It Works

**Goal:** Remove uncertainty. Show it's simple and low-commitment.

Three steps:

1. **Gesprek** — 90-minuten sessie. Jan komt langs of remote. Processen, tools en team doorlopen.
2. **Analyse** — Jan verwerkt inzichten tot concreet rapport met geprioriteerde kansen.
3. **Actieplan** — 30-minuten debrief. Resultaten doorlopen, eerste stap bepalen.

- **Format:** Horizontal 3-column (desktop) or vertical timeline (mobile). Numbered steps with clear labels.

### 6. Over Jan

**Goal:** Seal trust. Person, not company.

- **Photo of Jan** (professional but approachable)
- **First-person bio:**

  "Ik ben Jan Vaes. Ik leid de AI-adoptie bij een HR Tech bedrijf met 100+ medewerkers. Ik implementeer AI-workflows bij hun dochterbedrijf. Ik geef workshops over tools als Gemini en NotebookLM. En ik bouw AI-chatbots voor klanten.

  Ik vertel bedrijven niet wat AI theoretisch zou kunnen. Ik laat zien wat het concreet doet -- omdat ik het elke dag zelf doe."

- **No bullet lists of credentials.** Paragraph form, direct, repeated "Ik" structure for rhythm.
- Company names omitted for now (need permission). Can be added later.
- Optional future addition: small trust bar with client logos below the bio.

### 7. Contact (CTA)

**Goal:** Dead simple to reach out.

- **Section title:** "Klaar om te beginnen?" or "Laten we praten"
- **Subline:** "Vul het formulier in en ik neem binnen 24 uur contact op."
- **Form fields:**
  - Naam (required)
  - Bedrijf (required)
  - E-mail (required)
  - Telefoon (optional)
  - Bericht (optional)
- **Submit button:** Gold accent, "Verstuur"
- Max 5 fields. Every extra field kills conversion.

### 8. Footer

Minimal:
- Arize Consulting logo (small wordmark)
- Jan's email address
- LinkedIn link
- KBO/BTW-nummer (Belgian legal requirement)
- Copyright 2026 Arize Consulting

## Visual Design Direction

- **Colors:** Navy (#2B3044) primary, Gold (#D4993D) accent, White background, light warm grey for alternating sections
- **Typography:** Clean sans-serif. One font family, weight variations for hierarchy. (Inter, or similar)
- **Layout:** Generous whitespace, single-column content flow, max-width container
- **Style:** Minimal, modern, typography-driven. Inspiration: Linear, Stripe, Notion — but warmer/more personal given the Flemish B2B context
- **No stock photos.** Only Jan's photo and the logo.
- **Subtle animations:** Fade-in on scroll for sections. Nothing flashy.

## Technical Architecture

- **Single HTML file** with Tailwind CSS via CDN
- **No framework, no build step** — ship fast, host anywhere
- **Responsive / mobile-first** — visitors will likely arrive via LinkedIn on mobile
- **Contact form:** Formspree (or similar no-backend service), submissions forwarded to Jan's email
- **Hosting:** Netlify, Vercel, or any static host. Domain TBD.
- **Semantic HTML** — proper heading hierarchy, sections, labels on form fields
- **Accessibility:** Sufficient color contrast (navy/gold on white passes WCAG AA), focus states on interactive elements, alt text on images

## Assets Required

- Arize logo files (icon + wordmark) — exist, provided as images
- Professional photo of Jan — needed before launch
- Favicon — derive from the "A" icon logo

## Out of Scope

- Multi-language support (English version)
- Self-serve assessment (online tool, future product)
- Pricing display
- Blog or content pages
- Client logos / named case studies (pending permission)
- COO consulting as a service offering
- Implementation services
- CMS or admin panel
- Analytics (can be added later: simple Plausible or similar)

## Verification

- Page loads correctly on mobile (Chrome DevTools responsive mode)
- Contact form submits successfully and email arrives
- All sections visible and properly ordered
- Logo renders correctly
- Scroll anchors work from nav
- Color contrast passes WCAG AA check
- No horizontal scroll on mobile
- Footer contains required Belgian legal info (KBO/BTW)
