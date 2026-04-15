# Phase 3.5 — Pilot Migration

## Summary
Migrated 3 sample pages (one per archetype) to da.live. All content uploaded successfully (HTTP 201) and verified accessible (HTTP 200).

## Pilot Pages
| Archetype | Source URL | da.live Status | Preview Status |
|-----------|-----------|----------------|----------------|
| landing | /nl | ✅ 201/200 | ⚠️ Requires Code Sync |
| treatment | /nl/treatment/lips | ✅ 201/200 | ⚠️ Requires Code Sync |
| utility | /nl/contact-us | ✅ 201/200 | ⚠️ Requires Code Sync |

## Content Structure
### Homepage (/nl)
- Hero with JUVÉDERM key visual
- Intro section (default content)
- Why JUVÉDERM section with Cards block (4 value props)
- Before/After section with Columns block
- Treatment areas with Tabs block (VROUWELIJK/MANNELIJK)
- Clinic finder CTA

### Lips Treatment (/nl/treatment/lips)
- Hero with treatment image
- Intro with Cards block (3 value props)  
- Before/After with Columns block
- Product Carousel (3 products: VOLBELLA, VOLIFT, ULTRA 4)
- FAQ Accordion (4 questions)
- Clinic finder CTA

### Contact (/nl/contact-us)
- Simple default content with address and contact info

## Known Issue: Preview URLs
Preview URLs (aem.page) return 404 because the **AEM Code Sync GitHub App** has not been installed on the repository. This is a one-time setup step:
1. Visit https://github.com/apps/aem-code-sync/installations/new
2. Grant access to `jmffraiz/jv-test-2`
3. After installation, preview URLs will work automatically

## Tier 1 Validation
- **Result**: PASS (with degraded acceptance for preview URLs)
- **Fallback**: Content verified on da.live directly
