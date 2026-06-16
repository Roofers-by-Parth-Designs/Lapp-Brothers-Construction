# 00_IMPLEMENTATION_.md - Business Name, Location, Phone & City Replacement

This document outlines the steps to replace placeholders in `index.html` with business-specific details: `Lapp Brothers Construction`, `Winchester, TN`, `(931) 308-5617`, and local cities (`Winchester`, `Decherd`, `Estill Springs`).

## Checklist

- [x] Ask the user about hero name layout/formatting preference (completed via /grill-me)
- [x] Ask the user about review cities layout/formatting preference (completed via /grill-me)
- [x] Receive approval on the implementation plan
- [x] Replace `[Business Name]` in `index.html` (5 occurrences)
  - [x] Page Title (`<title>`)
  - [x] Navigation Logo (`.nav-logo`)
  - [x] Hero Heading (`.hero-name`)
  - [x] Customer Review Card text
  - [x] Footer (`.footer-name`)
- [x] Replace `[City, State]` in `index.html` (2 occurrences)
  - [x] Hero Eyebrow (`.hero-eyebrow`)
  - [x] Footer Note (`.footer-note`)
- [x] Replace `[Year]` in `index.html` (1 occurrence) with `2011`
  - [x] Hero Eyebrow (`.hero-eyebrow`)
- [x] Replace Phone Number placeholders in `index.html` (2 occurrences)
  - [x] Navigation Phone link (`.nav-phone`)
  - [x] CTA button (`.btn-white`)
- [x] Replace `[City]` in Recent Work section (3 occurrences)
  - [x] Caption 1 with `Winchester`
  - [x] Caption 2 with `Decherd`
  - [x] Caption 3 with `Estill Springs`
- [x] Replace `[City]` in Reviews section (3 occurrences)
  - [x] Review 1 text with `Winchester`
  - [x] Review 1 author city with `Winchester`
  - [x] Review 2 author city with `Decherd`
- [x] Verify the page layout and visual appearance

## Confirmed Design Decisions

- **Hero Title Split**: Confirmed layout is to place "Lapp Brothers" on the first line and "Construction" on the second line (italicized).
- **Location Replacement**: Replace `[City, State]` with `Winchester, TN`.
- **Year Replacement**: Replace `[Year]` with `2011`.
- **Phone Number Replacement**: Replace all `(000) 000-0000` texts with `(931) 308-5617` and `tel:+10000000000` with `tel:+19313085617`.
- **Recent Work Cities**: Replace `[City]` in the Recent Work section captions sequentially with `Winchester`, `Decherd`, and `Estill Springs`.
- **Review Section Cities**: Replace `[City]` in Review 1 (Mike T.) with `Winchester`, and in Review 2 (Sarah M.) with `Decherd`.

## Proposed Changes

### Lapp-Brothers-Construction

#### [MODIFY] [index.html](../index.html)

##### 1. Document Title (Line 6)
- **Before**: `<title>[Business Name] | Professional Roofing</title>`
- **After**: `<title>Lapp Brothers Construction | Professional Roofing</title>`

##### 2. Navigation Logo (Line 502)
- **Before**: `<span class="nav-logo">[Business Name]</span>`
- **After**: `<span class="nav-logo">Lapp Brothers Construction</span>`

##### 3. Hero Title (Lines 516-519)
- **Before**:
  ```html
  <h1 class="hero-name">
    [Business<br>
    <em>Name]</em>
  </h1>
  ```
- **After**:
  ```html
  <h1 class="hero-name">
    Lapp Brothers<br>
    <em>Construction</em>
  </h1>
  ```

##### 4. Hero Eyebrow (Line 515)
- **Before**: `<div class="hero-eyebrow">Serving [City, State] Since [Year]</div>`
- **After**: `<div class="hero-eyebrow">Serving Winchester, TN Since 2011</div>`

##### 5. Navigation Phone (Line 504)
- **Before**: `<a href="tel:+10000000000" class="nav-phone">(000) 000-0000</a>`
- **After**: `<a href="tel:+19313085617" class="nav-phone">(931) 308-5617</a>`

##### 6. Recent Work Image 1 Caption (Line 604)
- **Before**: `<div class="work-caption">Active Roof Installation & Framing — [City]</div>`
- **After**: `<div class="work-caption">Active Roof Installation & Framing — Winchester</div>`

##### 7. Recent Work Image 2 Caption (Line 609)
- **Before**: `<div class="work-caption">Detailed Shingle & Pipe Boot Repair — [City]</div>`
- **After**: `<div class="work-caption">Detailed Shingle & Pipe Boot Repair — Decherd</div>`

##### 8. Recent Work Image 3 Caption (Line 614)
- **Before**: `<div class="work-caption">Complete Residential Shingle Roofing — [City]</div>`
- **After**: `<div class="work-caption">Complete Residential Shingle Roofing — Estill Springs</div>`

##### 9. Review 1 Text (Line 628)
- **Before**: `...Best roofer in [City]. Fast, professional...`
- **After**: `...Best roofer in Winchester. Fast, professional...`

##### 10. Review 1 Author (Line 629)
- **Before**: `<div class="reviewer">— Mike T., [City]</div>`
- **After**: `<div class="reviewer">— Mike T., Winchester</div>`

##### 11. Review 2 Text (Line 634)
- **Before**: `...[Business Name] was the only one...`
- **After**: `...Lapp Brothers Construction was the only one...`

##### 12. Review 2 Author (Line 636)
- **Before**: `<div class="reviewer">— Sarah M., [City]</div>`
- **After**: `<div class="reviewer">— Sarah M., Decherd</div>`

##### 13. CTA Button Phone (Line 647)
- **Before**: `<a href="tel:+10000000000" class="btn-white">Call (000) 000-0000</a>`
- **After**: `<a href="tel:+19313085617" class="btn-white">Call (931) 308-5617</a>`

##### 14. Footer Name (Line 652)
- **Before**: `<span class="footer-name">[Business Name] Roofing</span>`
- **After**: `<span class="footer-name">Lapp Brothers Construction Roofing</span>`

##### 15. Footer Note (Line 653)
- **Before**: `<span class="footer-note">Licensed & Insured &nbsp;·&nbsp; [City, State]</span>`
- **After**: `<span class="footer-note">Licensed & Insured &nbsp;·&nbsp; Winchester, TN</span>`
