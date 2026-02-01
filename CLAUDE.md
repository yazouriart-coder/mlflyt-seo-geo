# CLAUDE.md - AI Assistant Guide for mlflyt-seo-geo

## Project Overview

This is a **static HTML/Markdown repository** for **MLflyt** (mlflyt.dk), a moving company based in Aarhus, Denmark with 32+ years of experience. The repository serves two purposes:

1. **SEO documentation** - Audit reports, action plans, competitive analysis, and technical fix specifications for improving the website's search engine performance.
2. **Ready-to-deploy landing pages** - GEO-targeted HTML pages optimized for local SEO (Skanderborg, Randers, etc.).

There is also legal documentation related to a contract dispute with an SEO agency.

**Client:** MLflyt / Khalil Yazouri
**Domain:** mlflyt.dk
**Language:** Danish (da)
**Brand mascot:** Giraffe (girafbiler)

---

## Repository Structure

```
mlflyt-seo-geo/
├── CLAUDE.md                           # This file - AI assistant guide
├── index.html                          # Navigation hub linking all documents
├── flyttefirma-skanderborg.html        # GEO landing page - Skanderborg
├── flyttefirma-randers.html            # GEO landing page - Randers
├── Brev_til_Advokat.html               # Legal letter to lawyer (contract dispute)
├── Dokumentation_Advokat.html          # Detailed legal documentation with evidence
├── SEO_RAPPORT_30-01-2026.md           # Full SEO audit report (30 Jan 2026)
├── HANDLINGSPLAN.md                    # 6-phase SEO action plan with timeline
├── SEO_FIXES.md                        # Specific technical SEO fixes with code
├── BUREAU_ANALYSE.md                   # SEO agency performance/financial analysis
└── KONKURRENCEANALYSE.md               # Competitive analysis of 5 rival companies
```

### File Categories

| Category | Files | Purpose |
|----------|-------|---------|
| Landing pages | `flyttefirma-skanderborg.html`, `flyttefirma-randers.html` | Deploy-ready GEO pages for mlflyt.dk |
| Navigation | `index.html` | Document hub with links to all files |
| SEO analysis | `SEO_RAPPORT_*.md`, `SEO_FIXES.md`, `HANDLINGSPLAN.md`, `KONKURRENCEANALYSE.md`, `BUREAU_ANALYSE.md` | Audit reports and action plans |
| Legal | `Brev_til_Advokat.html`, `Dokumentation_Advokat.html` | Contract dispute documentation |

---

## Technology Stack

- **HTML5** with semantic markup
- **CSS3** embedded in `<style>` tags (no external stylesheets)
- **JSON-LD** Schema.org structured data (MovingCompany / LocalBusiness)
- **Markdown** for reports and documentation
- **No build system** - pure static files, no npm/Node.js/bundling
- **No JavaScript framework** - vanilla HTML/CSS only
- **No tests** - no testing framework configured
- **Git** for version control (manual deployment assumed)

---

## Code Conventions

### HTML Structure

All landing pages follow this template pattern:

```html
<!DOCTYPE html>
<html lang="da">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>[Keyword] | 32+ Års Erfaring | MLflyt 🦒</title>
    <meta name="description" content="...">
    <meta name="keywords" content="...">
    <link rel="canonical" href="https://mlflyt.dk/[filename]">
    <!-- Open Graph tags -->
    <style>/* Embedded CSS */</style>
</head>
<body>
    <h1>[Keyword] 🦒</h1>
    <!-- Trust signals section -->
    <!-- Feature sections -->
    <!-- FAQ section -->
    <!-- Schema.org JSON-LD -->
    <!-- CTA -->
    <!-- Footer with internal links -->
</body>
</html>
```

### CSS Conventions

- **Color scheme:** `#1a365d` (dark blue, primary), `#ed8936` (orange, accent/CTA)
- **Background:** `#f7fafc` (light gray for feature boxes)
- **Text color:** `#718096` (secondary/muted text)
- **Font:** Arial, sans-serif (landing pages) / Times New Roman (legal docs)
- **Layout:** `max-width: 800px; margin: 0 auto;` centered single-column
- **Feature boxes:** Left border accent with `border-left: 4px solid #ed8936`
- **CTA buttons:** `.cta` class - orange background, white text, rounded corners
- **Flexbox** for trust signal rows
- **Print-friendly** `@media print` styles in legal documents

### SEO Conventions

- Every landing page must include:
  - Canonical URL (`<link rel="canonical">`)
  - Open Graph meta tags (`og:title`, `og:description`, `og:image`)
  - Meta description (max 160 chars, include USPs)
  - Title tag (max 60 chars, format: `[Keyword] | 32+ Års Erfaring | MLflyt 🦒`)
  - H1 with primary keyword and giraffe emoji
  - Schema.org JSON-LD (`MovingCompany` type)
  - FAQ section for featured snippets
  - Trust signals: Trustpilot 4.8/5, 32+ years, 10,000+ moves

### Schema.org Pattern

```json
{
  "@context": "https://schema.org",
  "@type": "MovingCompany",
  "name": "MLflyt",
  "image": "https://mlflyt.dk/logo.png",
  "address": {
    "@type": "PostalAddress",
    "addressLocality": "[City]",
    "addressCountry": "DK"
  },
  "areaServed": ["Aarhus", "Skanderborg", "Randers"],
  "aggregateRating": {
    "@type": "AggregateRating",
    "ratingValue": "4.8"
  }
}
```

### Markdown Conventions (Reports)

- Danish language throughout
- Emoji prefixes for section headers (e.g., `## 🚨 KRITISKE FEJL`)
- Tables for structured comparisons
- Checkbox lists `- [ ]` for action items
- Status indicators: ✅ (good), ❌ (bad/missing), ⚠️ (warning/needs attention)
- Code blocks with `html` or `json` syntax highlighting for technical examples

---

## Naming Conventions

- **GEO landing pages:** `flyttefirma-[city].html` (lowercase, hyphenated)
- **Reports:** `UPPERCASE_NAME.md` (e.g., `SEO_FIXES.md`, `HANDLINGSPLAN.md`)
- **Legal docs:** `CamelCase_Name.html` (e.g., `Brev_til_Advokat.html`)
- **CSS classes:** lowercase, descriptive (`.cta`, `.feature`, `.trust`, `.faq`)

---

## Key Business Context

When creating or modifying content for MLflyt, keep these in mind:

- **Brand name:** MLflyt (capital M, capital L)
- **Correct spelling:** "Aarhus" (NOT "Aahrus" - this was a critical SEO bug)
- **USPs:** 32+ years experience, iconic giraffe trucks (girafbiler), Trustpilot 4.8/5
- **Service areas:** Aarhus, Skanderborg, Randers (primary); Risskov, Aarhus C (secondary)
- **Services:** Moving (flytning), packing (pakning), storage (opbevaring)
- **Competitors:** Jysk Flyttefirma, Aarhus Flytteservice, Flyttebanden, AKL Flyt
- **Related business:** AK Affaldsservice (waste management)
- **Primary keyword targets:** "flyttefirma aarhus", "flyttefirma skanderborg", "flyttefirma randers"

---

## Creating New GEO Landing Pages

When adding a new city-specific landing page:

1. Copy an existing GEO page (e.g., `flyttefirma-skanderborg.html`) as template
2. Replace city name throughout (title, h1, meta tags, body text, Schema.org)
3. Update canonical URL to `https://mlflyt.dk/flyttefirma-[city].html`
4. Update Open Graph tags with city-specific content
5. Customize FAQ section with locally relevant questions
6. Update Schema.org `areaServed` to include the new city
7. Add link to the new page in `index.html`
8. Ensure title is max 60 characters: `Flyttefirma [City] | 32+ Års Erfaring | MLflyt 🦒`

---

## Deployment

There is no automated build or CI/CD pipeline. Files are:

- Static HTML/CSS ready for direct upload to mlflyt.dk
- Markdown reports are reference documentation (not deployed to web)
- Git is used for version control only
- Deployment is manual (assumed FTP/SFTP or hosting panel upload)

---

## Git Conventions

- **Commit messages:** Danish language, descriptive (e.g., "Tilføjet index.html")
- **Author:** Mujaffa (khalilyazouri@gmail.com)
- No branch strategy beyond main development
- No CI/CD hooks or automated checks

---

## Known Issues & Active Work

Per the SEO audit (30 Jan 2026):

1. **CRITICAL:** The live site mlflyt.dk has "Aahrus" typo in title tag
2. Title tag is 105 chars (should be max 60)
3. H1 tag is generic ("Velkommen til MLflyt") - needs keyword optimization
4. Missing Schema.org markup on live site
5. Missing canonical URLs on live site
6. Missing Open Graph tags on live site
7. No GEO pages for Aarhus C or Risskov yet
8. No blog/content marketing section yet
