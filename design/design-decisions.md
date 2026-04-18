# Design Decisions — BAR.BOOK

A record of the key design decisions made during this project, the reasoning behind them, and the alternatives considered.

---

## Navigation Model

**Decision:** Bottom navigation bar with 4 persistent tabs (Discover, Reservations, Saved, Profile).

**Rationale:** Mobile users expect bottom navigation on iOS and Android. Four tabs keeps primary actions visible without overwhelming the UI. A top app bar handles in-flow navigation (back arrows, search, contextual actions).

**Alternatives considered:**
- Hamburger/drawer menu — dismissed because it hides primary actions and increases tap depth
- Tab bar at top — dismissed as it conflicts with native platform conventions

---

## Filter Chips on Search Screen (Not in a Modal)

**Decision:** Dietary and ambiance filters appear as horizontal-scrolling chips directly on the search screen, not inside a filter modal.

**Rationale:** Research showed that every additional tap to access filters caused users to lose momentum. Visible chips create immediate discoverability and reduce the filter flow from 4 taps (tap filter icon → open modal → select → apply) to 1 tap (tap chip).

**Alternatives considered:**
- Full-screen filter modal (common pattern) — dismissed after testing showed users abandoned the flow before applying filters
- Floating filter button — dismissed as it obscures results and requires an extra step

---

## Colour Palette — Mauve as Primary Brand Colour

**Decision:** `#BF8DBC` (muted mauve/rose) as the primary brand accent.

**Rationale:** The food discovery space is dominated by reds and oranges (appetite stimulation — Yelp, DoorDash). A warm, sophisticated mauve differentiates BAR.BOOK and signals a more considered, curated experience. It reads as warm and inviting without being aggressive.

**Teal (`#557174`)** was chosen as a secondary accent specifically to encode dietary/vegan content — green connotes nature and plant-based food, while the muted teal keeps it within the palette's sophistication register.

---

## Typography — Playfair Display + DM Sans

**Decision:** Playfair Display (serif) for display headings and app name; DM Sans for all body and UI text.

**Rationale:** The serif/sans pairing creates a clear typographic hierarchy and gives the app an editorial, curated quality — more like a food magazine than a utility app. Playfair's high contrast strokes give the BAR.BOOK wordmark immediate personality.

**Alternatives considered:**
- All-sans (clean, minimal) — felt generic for the brand context
- Custom rounded sans — would require more design work without sufficient benefit at MVP stage

---

## Saving Venues — Heart Icon vs. "Save" Button

**Decision:** A heart icon on the venue detail card, upgraded to a labelled "Save" button after usability testing revealed the icon alone was missed by 20% of users.

**Rationale:** The heart icon is universally understood on social media, but in a booking context, users are more task-focused and scan less carefully. Adding a text label removes ambiguity while keeping the icon for quick recognition.

**Lesson learned:** Familiar icons in unfamiliar contexts need supporting labels. This is a core accessibility principle that testing reinforced empirically.

---

## Onboarding — 3 Slides, No Registration Wall

**Decision:** A 3-slide value proposition onboarding carousel before the login screen, with the option to skip to login directly.

**Rationale:** Research showed that users want to understand what an app does before committing to registration. Three slides cover the three core values: Discover, Reserve, Save. A skip option respects returning users' time.

**The 3 propositions chosen:**
1. Find the perfect gastronomic spot (discovery value)
2. Reserve and never wait again (convenience value)
3. Save venues you love, for later (retention value)

---

## Reservation Form — Minimal Fields

**Decision:** Reservation form contains only: Date, Time, Party Size, and optional Notes. No payment at this stage.

**Rationale:** For the MVP, the goal is to validate the booking flow. Payment adds friction and complexity that is out of scope. Keeping the form to 4 fields (3 required, 1 optional) reduces cognitive load and maximises completion rate.

**Future consideration:** Add payment for venues that require deposits for large group reservations.

---

## Category Icons — Contained vs. Bare

**Decision:** Category icons appear both bare (in navigation) and contained in circular backgrounds (in category chip selectors on the search screen).

**Rationale:** Bare icons work where context is clear (bottom navigation). In category chips, the circular container creates a visual target that is easier to tap and scan. The size difference (18px bare vs. 48px contained) reflects the gestural hierarchy — exploration actions deserve larger targets.

---

## Atomic Design — Component Hierarchy

The design system follows Atomic Design principles:

| Level | Examples |
|-------|---------|
| **Atoms** | Colour tokens, type styles, icons, toggle switch |
| **Molecules** | Search bar, filter chip, venue card, reservation field |
| **Organisms** | Search results list, bottom navigation, reservation form |
| **Templates** | Venue discovery screen, booking flow screen |
| **Pages** | Onboarding, home, venue detail, confirmation |

This structure ensures every component is reusable, documented, and ready for developer handoff.
