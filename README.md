# BAR.BOOK — UX/UI Case Study

> A gastronomic venue discovery and reservation mobile app designed for diverse dining needs.

**[→ View Live Portfolio Case Study](https://your-username.github.io/barbook-ux-casestudy)**  
**[→ View Figma Prototype](https://www.figma.com/design/QZsJyIFc6EkSKf1G9WcuQc/UX-UI-Miriam)**

---

## Overview

BAR.BOOK is a mobile app concept that lets users search, filter, and reserve tables at gastronomic venues — with a strong focus on dietary inclusivity (vegan, vegetarian, gluten-free) and group coordination.

This repository contains the complete UX/UI design documentation for the project, structured as a professional portfolio case study.

| | |
|---|---|
| **Role** | UX/UI Designer (solo project) |
| **Platform** | iOS & Android |
| **Duration** | 4 months |
| **Tools** | Figma · Miro |
| **Methods** | User Interviews · Competitive Analysis · Affinity Mapping · Wireframing · Usability Testing |

---

## The Problem

Finding a restaurant that works for everyone — especially in mixed groups with dietary restrictions — requires juggling multiple apps. No single platform combines smart filtering, menu information, and table reservations.

> *"I'm the one who always has to suggest places — and I never know which ones are vegan-friendly."*  
> — Research participant

---

## Design Process

```
Empathise → Define → Ideate → Prototype → Test
```

### 1. Research
- 8 semi-structured user interviews
- Competitive benchmarking of Google Maps, TripAdvisor, OpenTable
- 60+ insights clustered via affinity mapping

### 2. User Personas

| Persona | Profile | Core Need |
|---------|---------|-----------|
| **Agustín, 27** | Marketing professional | Always needs a venue ready to suggest to his group |
| **Micaela, 24** | Tourism student | Discovers culturally diverse venues, needs bike infrastructure |
| **Claudia, 38** | Teacher | Finds vegetarian-friendly places that don't exclude her |

### 3. Define — POV & MVP

**How Might We:**
> How might we help diverse groups of diners — each with different dietary needs and social contexts — find, evaluate, and reserve the right gastronomic venue in a single, seamless experience?

**MVP Core Features:**
- Smart search with dietary and ambiance filters
- In-app table reservation (date, time, party size)
- Save venues to a personal favourites list
- View and manage reservation history

### 4. Information Architecture

```
Launch           Discover          Evaluate          Reserve           Manage
──────────       ──────────        ──────────        ──────────        ──────────
Onboarding   →  Search + Filter → Venue Detail   → Book Table     → My Reservations
Login/Register  Results List      Photos · Menu     Date/Time/Party   Saved Venues
```

**Navigation:** Bottom tab bar (Discover · Reservations · Saved · Profile) + Top app bar with contextual search.

### 5. Design System

**Colour Palette:**

| Token | Hex | Usage |
|-------|-----|-------|
| Mauve | `#BF8DBC` | Primary brand, CTAs, active states |
| Ink | `#242424` | Typography, dark backgrounds |
| Teal | `#557174` | Vegan/dietary tags, secondary accents |
| Fog | `#F5F2F0` | Backgrounds, cards |

**Typography:**
- Display: Playfair Display (headings, app name)
- Body: DM Sans (all UI text)
- Mono: DM Mono (labels, metadata, tags)

**Key Components:** Search bar · Filter chips · Bottom navigation · Venue cards · Switches · Reservation form

### 6. Usability Testing

Moderated sessions with 5 participants using a clickable Figma prototype.

**Test Scenario:** Plan a birthday celebration for 8 people (vegan-friendly, outdoor seating).

**Results:**

| Task | Completion | Notes |
|------|------------|-------|
| Search, filter & reserve | ✅ 100% | All users completed on first attempt |
| Log in | ✅ 100% | No friction observed |
| Save a venue | ⚠️ 80% | Heart icon needs higher contrast |
| View reservations | ⚠️ 60% | Tab label not immediately obvious |

**Key Improvements Identified:**
- Increase contrast on the save/heart icon
- Add text labels to bottom navigation icons
- Surface party-size as a top-level filter chip (not just inside detail view)

---

## Key Learnings

1. **Dietary filters are primary, not secondary** — placing them front and centre changed the entire emotional experience
2. **Icons without labels cause hesitation** — hybrid icon + label approach sped up task completion
3. **Confirmation screens build trust** — a clear success state was the most impactful single screen
4. **Filtering must be fast** — chips on the search screen reduced the filter flow from 4 taps to 1
5. **Realistic scenarios surface real anxiety** — using a birthday context revealed emotional friction points abstract tasks miss
6. **Saved lists create return visits** — a retention insight that emerged purely from observing user behaviour

---

## Next Steps

- **Phase 1 (Immediate):** Iterate on usability findings and re-test
- **Phase 2 (Short-term):** Expand dietary filter taxonomy, full menu integration
- **Phase 3 (Medium-term):** Social features — share options, group voting, reservation reminders

---

## Repository Structure

```
barbook-ux-casestudy/
├── docs/
│   └── index.html          # Live portfolio case study (GitHub Pages)
├── research/
│   └── research-plan.md    # Interview guide & research objectives
├── design/
│   └── design-decisions.md # Key design decisions & rationale
├── CHANGELOG.md            # Version history
└── README.md               # This file
```

---

## How to View Locally

```bash
git clone https://github.com/your-username/barbook-ux-casestudy.git
cd barbook-ux-casestudy
open docs/index.html
```

Or simply open `docs/index.html` in any browser — no build step required.

---

## Deploying to GitHub Pages

1. Push this repository to GitHub
2. Go to **Settings → Pages**
3. Set source to **Deploy from a branch → `main` → `/docs`**
4. Your case study will be live at `https://your-username.github.io/barbook-ux-casestudy`

---

## About

Designed by **Miriam Costa Manticof** — UX/UI Designer  
[Portfolio](#) · [LinkedIn](#) · [Figma](https://www.figma.com/design/QZsJyIFc6EkSKf1G9WcuQc/UX-UI-Miriam)

---

*This case study was designed as part of a UX/UI design program. All user research data has been anonymised.*
