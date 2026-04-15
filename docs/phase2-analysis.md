# Phase 2 — Analysis Report

## Site: https://www.juvederm.nl
## Date: 2026-04-15

## Phase 2a — Scrape Samples

Scraped all 11 pages using Playwright with full-page screenshots and cleaned HTML.

### Pages Scraped Per Archetype

| Archetype | Pages Scraped | Status |
|-----------|--------------|--------|
| homepage | 2 (desktop + mobile) | ✅ |
| treatment | 5 (lips, enhance, male, eye-area, restore) | ✅ |
| faq | 2 (desktop + mobile) | ✅ |
| find-a-clinic | 2 (desktop + mobile) | ✅ |
| legal | 3 (contact-us, disclaimer, terms) | ✅ |

### Notes
- Site uses Adobe Dynamic Media for images (dm-aid-based URLs)
- AEM component-based rendering with experience fragments for header/footer
- SSL cert issues required `ignoreHTTPSErrors` and custom user agent in Playwright

## Phase 2b — Block Inventory

### Block Collection Matches
All 7 blocks sourced from Adobe AEM Block Collection:

| Block | Source | Purpose |
|-------|--------|---------|
| hero | block-collection | Full-width hero with image, heading, CTA |
| cards | block-collection | Grid of feature items with icons/text |
| columns | block-collection | Side-by-side content layouts |
| accordion | block-collection | Expandable Q&A sections |
| tabs | block-collection | VROUWELIJK/MANNELIJK tabbed content |
| carousel | block-collection | Product carousel on treatment pages |
| fragment | block-collection | Shared/reusable content sections |

### No Custom Blocks Required
All site patterns map cleanly to existing Block Collection blocks.

## Phase 2c — Blueprint

### Archetype Blueprints

**Homepage**: hero → why-juvederm (cards) → before/after (carousel) → treatment tabs → clinic finder → references

**Treatment** (5 pages): hero → intro features (cards) → before/after (columns) → products (carousel) → FAQ (accordion) → treatment tabs → clinic finder → references

**FAQ**: hero → multiple Q&A sections (columns with image + text) → references

**Find-a-clinic**: heading + search CTA + city links (columns)

**Legal**: Simple default content (headings, paragraphs, lists)

### Site Conventions
- Language: Dutch (nl-NL)
- Path prefix: /nl/
- Mandatory regulatory disclaimer on all pages
- Reference footnotes on treatment/FAQ pages
- Product trademark symbols (®) must be preserved
- Before/after images labeled Voor/Na

## Validation
- Phase 2a Tier 1: ✅ PASS
- Phase 2b Tier 1: ✅ PASS
- Phase 2c Tier 1: ✅ PASS
