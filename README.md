# Según tu Palabra — pitch deck (preview: slides 1–3)

Interactive HTML pitch deck, built as a single self-contained page (`index.html`).
Open it directly in a browser, or serve the folder (e.g. `npx http-server .`).

This is the **first pass** requested before building the remaining 8 slides:
system + concept + slides 1–3 only, for review.

## Navigation

- Click the right/left half of the screen, or the ‹ › buttons, or `→` / `space` / `←`.
- Each slide advances through 2–3 "beats" (entrance → development → transformation)
  before moving to the next slide, so the pace can be matched to the spoken pitch.
- The top segmented bar (11 segments, echoing the app's own onboarding-screen
  progress bar) shows true position in the full 11-slide deck, even though only
  slides 1–3 are built.

## Design system

**Palette** — ink navy `#14151C` (not pure black), paper `#FFFFFF`, a muted
steel blue `#33517E` (from the app's own gradient screens) for structure/kickers,
and a single warm spot color, terracotta `#BE4F2C`, spent in exactly one place
per slide (the emphasis word, the highlight sweep, the "break-even"-style
convergence node) — never as decoration.

**Type** — three roles, no font used outside its role:
- Display — **Bricolage Grotesque** (700/800): headlines, the giant wordmark,
  the seed-word statements. Has enough character to carry big type without
  tipping into a generic geometric sans.
- Body/UI — **IBM Plex Sans**: paragraphs, chips, buttons.
- Mono — **IBM Plex Mono**: kickers, tags, running-head, data-style labels
  (stat values, ruler labels). Signals "this is a number/label," not prose,
  and gives the deck a digital-product texture distinct from an editorial
  magazine's serif-mono pairing.

**Grid** — a fixed 1600×900 logical canvas (true 16:9), scaled to fit the
viewport like a real keynote, so every composition is hand-placed rather than
centered-text-on-empty-space. Consistent margins (96px sides, persistent
header/footer chrome) with fully asymmetric content per slide.

**Motion** — a single state-machine (`applyState(i)`) drives every slide;
"back" is just re-applying an earlier state, so rewinding is free and correct.
Reveals use clip-path curtains, staggered fades, and — for slide 2→3 — literal
shared elements: four words are *the same DOM nodes* in both slides, animated
from a scattered collage into the headline row. Nothing fades to black and
back; things become other things.

## Concept map — all 11 slides

Built so far: **1–3**. Sketched below for continuity/review before building on.

1. **Portada** — masthead-style cover. Wordmark, tagline, two grounding stats
   (5 modos · 500M+ hispanohablantes), ghost "1:1" verse-reference texture.
2. **Búsqueda** — the six real onboarding goals (from the reference screens)
   scattered as a collage, four of them typographically emphasized.
3. **Descubrimiento** — those four words migrate into a thesis statement;
   a converging "ruler" visualizes many paths → one book. Ends on a question.
4. **El problema (67%)** — giant `67%` as the composition's anchor; a
   100-unit grid that fills in as it's discussed; surrounding tags ("católicos",
   "Biblia", "raramente/nunca").
5. **Los 5 modos** — Etimológico / Cristológico / Histórico / Pastoral /
   Lectio Divina, scattered; selecting one expands it and shows a sample of
   its output, with an "IA" layer visually connecting all five.
6. **La app** — a simulated phone, zoom-in → real interaction (home → capítulo
   → pasaje → elegir modo → contenido generado → volver → otro modo) → zoom-out.
7. **El mercado** — España + Hispanoamérica map filling in progressively,
   counter climbing toward ~500M, labels appearing at real locations.
8. **El modelo de negocio** — the map resolves into a simple structural
   diagram (the transition motif: map → line).
9. **Finanzas** — CONSERVADOR/REALISTA toggle that *morphs* the curve rather
   than swapping it; scrubbing shows month-by-month ingresos/gastos/resultado;
   break-even gets its own small animation.
10. **Inversión** — the financial curve resolves into the `200.000 €` ask and
    a use-of-funds breakdown.
11. **Cierre** — everything clears back to a minimal closing screen, mirroring
    slide 1.

## Open items before slides 4–11

- **Script/copy**: slides 1–3 use placeholder copy written to match the
  brief's narrative beats (búsqueda → descubrimiento) and the real onboarding
  content from the reference screenshots. The 67%, mercado, and finanzas
  slides need the actual figures/copy from the source deck.
- **Financial interactive panel**: the brief references an HTML panel to
  match the interaction level of for slide 9 — not yet received in this
  session. Needed before that slide can be built for real (chart shape,
  exact scenario numbers, break-even month).
- **App screenshots/flow**: slide 6's simulated phone will look most
  convincing built from the actual current screens of the app (or high-fidelity
  descriptions of each) rather than re-imagined ones.
