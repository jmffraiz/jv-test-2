# Phase 2 — Analysis

## Summary
Analyzed 11 pages across 3 archetypes. Identified 6 blocks for the palette.

## Archetypes (Consolidated)
| Archetype | Pages | Description |
|-----------|-------|-------------|
| landing | 2 | Homepage + FAQ - rich content landing pages |
| treatment | 5 | Treatment detail pages (lips, eyes, enhance, restore, male) |
| utility | 4 | Find-a-clinic, contact, disclaimer, terms |

## Block Palette
| Block | Source | Purpose |
|-------|--------|---------|
| hero | block-collection | Full-width hero with image + heading |
| cards | block-collection | Value proposition grid cards |
| carousel | block-collection | Product showcase carousel |
| columns | block-collection | Side-by-side content layout |
| accordion | block-collection | Expandable FAQ sections |
| tabs | block-collection | Treatment area tab switcher |

All 6 blocks sourced from the AEM Block Collection (Adobe-maintained).

## Site Conventions
- **Language**: Dutch (nl-NL)
- **Shared Sections**: Treatment tabs, clinic finder CTA, before/after comparison appear across multiple pages
- **Regulatory**: Medical disclaimer required on every page, numbered footnote references
- **Warning Banner**: Footer warning about aesthetic procedures (Dutch regulatory requirement)

## Content Modeling Decisions
- Value props → Cards block (collection model, 3-4 items per page)
- Product listings → Carousel block (scrollable on mobile)
- FAQ items → Accordion block (collection model)
- Before/after → Columns block (2-column layout)
- Gender tabs → Tabs block (auto-blocked from section headings)
- Most utility pages → Default content only (no blocks needed)

## Tier 1 Validation
- 2a (Scrape): PASS
- 2b (Inventory): PASS
- 2c (Blueprint): PASS
- Retries: 1 (restructured archetypes to ensure ≥ 2 pages each)
