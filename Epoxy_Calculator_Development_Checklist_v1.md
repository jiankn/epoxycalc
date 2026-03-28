# Epoxy Project Planner - Development Checklist v1

## 0. Goal
Build the full production site in one pass, based on [Epoxy_Calculator_PRD_v4.md](C:/Users/JKN/OneDrive/桌面/fsdownload/Epoxy_Calculator_PRD_v4.md).

Core rule:

**One page = one core search intent = one primary keyword cluster.**

The site should launch with:

- Full information architecture
- Reusable calculator and guide components
- Technical SEO completed
- Internal links completed
- AdSense / affiliate slots prepared without hurting UX

## 1. Global Build Checklist

### 1.1 Site Foundation
- [ ] Use SSR or SSG.
- [ ] Make sure core content exists in HTML on first response.
- [ ] Build a shared layout with header, footer, breadcrumb, and related-links area.
- [ ] Add a consistent visual system based on the V4 PRD.
- [ ] Build mobile-first, bright-theme-only UI.

### 1.2 Technical SEO
- [ ] Generate clean URLs exactly as defined in this doc.
- [ ] Add unique `title`, `meta description`, `H1`, canonical for every indexable page.
- [ ] Add `noindex` for parameter/state/filter URLs.
- [ ] Add `robots.txt`.
- [ ] Generate `sitemap-index.xml`.
- [ ] Generate `sitemap-calculators.xml`.
- [ ] Generate `sitemap-guides.xml`.
- [ ] Generate `sitemap-site.xml`.
- [ ] Add `BreadcrumbList` structured data across indexable pages.
- [ ] Add `Article` structured data on guide pages.

### 1.3 Trust / Site Quality Pages
- [ ] Build `/about`.
- [ ] Build `/authors`.
- [ ] Build `/methodology`.
- [ ] Build `/contact`.
- [ ] Build `/faq`.

### 1.4 Shared Content / UX Systems
- [ ] Shared calculator shell
- [ ] Shared result card
- [ ] Shared "Why this estimate changed" module
- [ ] Shared "Compare scenarios" module
- [ ] Shared "How to measure" module
- [ ] Shared "Common mistakes" module
- [ ] Shared FAQ block
- [ ] Shared related-links block
- [ ] Shared affiliate recommendation block
- [ ] Shared sticky mobile summary

### 1.5 Tracking
- [ ] Track page view
- [ ] Track first input
- [ ] Track calculation completed
- [ ] Track compare-scenarios usage
- [ ] Track FAQ open
- [ ] Track measurement-guide open
- [ ] Track affiliate CTA impression
- [ ] Track affiliate CTA click
- [ ] Track related-links click

## 2. Shared Module Library

Use these module IDs across page builds.

- `M01` Hero intro
- `M02` Calculator shell
- `M03` Unit toggle
- `M04` Project-type toggle
- `M05` Result card
- `M06` Why this estimate changed
- `M07` Compare scenarios
- `M08` How to measure
- `M09` Common mistakes
- `M10` Product type recommendation
- `M11` Affiliate CTA block
- `M12` FAQ block
- `M13` Formula / methodology summary
- `M14` Cost estimator
- `M15` Coverage / conversion quick table
- `M16` Guide answer summary
- `M17` Related links
- `M18` Sticky mobile summary
- `M19` Example projects
- `M20` Checklist block

## 3. Global Navigation

### 3.1 Header Nav
- [ ] Epoxy Calculator
- [ ] River Table
- [ ] Deep Pour
- [ ] Coverage
- [ ] Cost
- [ ] Converter
- [ ] Guides

### 3.2 Footer Nav
- [ ] Calculators
- [ ] Guides
- [ ] Methodology
- [ ] Authors
- [ ] FAQ
- [ ] Contact

## 4. Page Build Matrix

## 4.1 Hub / Head-Term Pages

### Page 01
- URL: `/`
- Primary intent: Find the main epoxy planning tool and site entry point
- Primary keyword cluster: `epoxy calculator`, `epoxy resin calculator`
- Title: `Epoxy Calculator & Resin Project Planner`
- H1: `Epoxy Calculator and Resin Project Planner`
- Meta description: `Estimate epoxy resin volume, coverage, waste, cost, and project-specific needs for river tables, deep pours, coatings, and more.`
- Modules: `M01 M17`
- Required sections:
  - Main value proposition
  - Primary entry to `/epoxy-calculator`
  - Entry cards to major scenario calculators
  - Short explanation of waste, coverage, and cost planning
  - FAQ teaser
- Internal links:
  - `/epoxy-calculator`
  - `/river-table-epoxy-calculator`
  - `/deep-pour-epoxy-calculator`
  - `/epoxy-coverage-calculator`
  - `/epoxy-unit-converter`

### Page 02
- URL: `/epoxy-calculator`
- Primary intent: Calculate general epoxy needs
- Primary keyword cluster: `epoxy calculator`
- Supporting variants: `epoxy resin calculator`, `how much epoxy do i need`
- Title: `Epoxy Calculator: Coverage, Volume & Cost Estimator`
- H1: `Epoxy Calculator`
- Meta description: `Use this epoxy calculator to estimate resin volume, coverage, waste, part A/B split, and project cost for common epoxy jobs.`
- Modules: `M01 M02 M03 M04 M05 M06 M07 M10 M11 M12 M13 M17 M18`
- Required sections:
  - General calculator
  - Result explanation
  - Quick links to scenario calculators
  - Formula summary
  - FAQ
- Internal links:
  - `/epoxy-coverage-calculator`
  - `/epoxy-volume-calculator`
  - `/how-much-epoxy-do-i-need`
  - `/epoxy-cost-calculator`
  - `/epoxy-unit-converter`

### Page 03
- URL: `/epoxy-coverage-calculator`
- Primary intent: Estimate surface coverage and coating thickness
- Primary keyword cluster: `epoxy coverage calculator`
- Supporting variants: `epoxy resin coverage calculator`
- Title: `Epoxy Coverage Calculator: How Much Resin You Need`
- H1: `Epoxy Coverage Calculator`
- Meta description: `Calculate epoxy coverage by surface size and thickness, with waste, edge soak-in, seal coat guidance, and product-type recommendations.`
- Modules: `M01 M02 M03 M05 M06 M10 M11 M12 M13 M15 M17 M18`
- Required sections:
  - Coverage calculator
  - Thickness examples
  - Waste guidance
  - Coverage quick table
- Internal links:
  - `/epoxy-calculator`
  - `/table-top-epoxy-calculator`
  - `/bar-top-epoxy-calculator`
  - `/countertop-epoxy-calculator`
  - `/epoxy-coverage-chart`

### Page 04
- URL: `/epoxy-volume-calculator`
- Primary intent: Calculate general epoxy volume
- Primary keyword cluster: `epoxy volume calculator`
- Supporting variants: `epoxy resin volume calculator`
- Title: `Epoxy Volume Calculator for Tables, Voids & Slabs`
- H1: `Epoxy Volume Calculator`
- Meta description: `Calculate epoxy volume for rectangular, round, and simple slab projects with unit conversion, waste guidance, and practical examples.`
- Modules: `M01 M02 M03 M05 M06 M12 M13 M15 M17`
- Required sections:
  - Shape selection
  - Rectangular and round formulas
  - Conversion examples
  - FAQ
- Internal links:
  - `/epoxy-calculator`
  - `/round-epoxy-table-calculator`
  - `/void-fill-epoxy-calculator`
  - `/epoxy-unit-converter`

## 4.2 Scenario Calculator Pages

### Page 05
- URL: `/river-table-epoxy-calculator`
- Primary intent: Estimate resin for river table / live edge projects
- Primary keyword cluster: `river table epoxy calculator`
- Supporting variants: `epoxy calculator for river table`, `live edge epoxy calculator`, `river table resin calculator`
- Title: `River Table Epoxy Calculator: Resin, Waste & Cost`
- H1: `River Table Epoxy Calculator`
- Meta description: `Estimate epoxy for river tables with quick mode, segment mode, waste buffer, seepage, cost, and deep-pour recommendations.`
- Modules: `M01 M02 M03 M04 M05 M06 M07 M08 M09 M10 M11 M12 M13 M14 M18 M19 M20`
- Required sections:
  - Quick mode
  - Segment mode
  - Cost output
  - How to measure irregular rivers
  - Mistakes and checklist
- Internal links:
  - `/how-much-epoxy-do-i-need-for-a-river-table`
  - `/how-to-measure-a-river-table-for-epoxy`
  - `/deep-pour-epoxy-calculator`
  - `/epoxy-cost-calculator`
  - `/deep-pour-vs-table-top-epoxy`

### Page 06
- URL: `/deep-pour-epoxy-calculator`
- Primary intent: Estimate deep pour projects and layer planning
- Primary keyword cluster: `deep pour epoxy calculator`
- Supporting variants: `deep pour resin calculator`
- Title: `Deep Pour Epoxy Calculator: Layers, Volume & Cost`
- H1: `Deep Pour Epoxy Calculator`
- Meta description: `Calculate deep pour epoxy volume, layer count, waste, and cost. Compare deep pour vs table top resin for thick casting projects.`
- Modules: `M01 M02 M03 M05 M06 M07 M09 M10 M11 M12 M13 M14 M18 M20`
- Required sections:
  - Max depth guidance
  - Layer recommendations
  - Compare scenarios
  - Product type decision help
- Internal links:
  - `/river-table-epoxy-calculator`
  - `/deep-pour-vs-table-top-epoxy`
  - `/epoxy-cost-calculator`
  - `/epoxy-mixing-ratio-guide`

### Page 07
- URL: `/table-top-epoxy-calculator`
- Primary intent: Estimate tabletop coating jobs
- Primary keyword cluster: `table top epoxy calculator`
- Supporting variants: `tabletop epoxy calculator`, `epoxy table top calculator`
- Title: `Table Top Epoxy Calculator for Coats & Pours`
- H1: `Table Top Epoxy Calculator`
- Meta description: `Estimate epoxy for tabletops and surface coats with coverage, thickness, waste, and top-coat recommendations.`
- Modules: `M01 M02 M03 M05 M06 M09 M10 M11 M12 M13 M15 M18`
- Required sections:
  - Coating thickness examples
  - Coverage logic
  - Product type recommendations
- Internal links:
  - `/epoxy-coverage-calculator`
  - `/bar-top-epoxy-calculator`
  - `/countertop-epoxy-calculator`
  - `/deep-pour-vs-table-top-epoxy`

### Page 08
- URL: `/bar-top-epoxy-calculator`
- Primary intent: Estimate bar top coating volume
- Primary keyword cluster: `bar top epoxy calculator`
- Supporting variants: `bar countertop epoxy calculator`
- Title: `Bar Top Epoxy Calculator for Resin Coats`
- H1: `Bar Top Epoxy Calculator`
- Meta description: `Calculate epoxy for bar tops with surface coverage, waste, edge soak-in, and finish-coat guidance for high-gloss pours.`
- Modules: `M01 M02 M03 M05 M06 M09 M10 M11 M12 M13 M15 M18`
- Required sections:
  - Coverage calculator
  - Edge and overage notes
  - Related top-coat examples
- Internal links:
  - `/table-top-epoxy-calculator`
  - `/countertop-epoxy-calculator`
  - `/epoxy-coverage-calculator`

### Page 09
- URL: `/countertop-epoxy-calculator`
- Primary intent: Estimate countertop resin needs
- Primary keyword cluster: `countertop epoxy calculator`
- Supporting variants: `epoxy countertop calculator`, `counter top epoxy calculator`
- Title: `Countertop Epoxy Calculator for Resin Coverage`
- H1: `Countertop Epoxy Calculator`
- Meta description: `Use this countertop epoxy calculator to estimate coverage, waste, thickness, and resin quantity for kitchen and surface projects.`
- Modules: `M01 M02 M03 M05 M06 M09 M10 M11 M12 M13 M15 M18`
- Required sections:
  - Surface project calculator
  - Thickness guidance
  - Coverage examples
- Internal links:
  - `/epoxy-coverage-calculator`
  - `/table-top-epoxy-calculator`
  - `/bar-top-epoxy-calculator`

### Page 10
- URL: `/garage-floor-epoxy-calculator`
- Primary intent: Estimate epoxy for garage floor coating
- Primary keyword cluster: `garage floor epoxy calculator`
- Supporting variants: `epoxy floor calculator`, `garage epoxy coverage calculator`
- Title: `Garage Floor Epoxy Calculator: Coverage & Kits`
- H1: `Garage Floor Epoxy Calculator`
- Meta description: `Estimate epoxy coverage, kit size, waste, and floor area for garage floor coatings with practical project planning guidance.`
- Modules: `M01 M02 M03 M05 M06 M09 M10 M11 M12 M13 M14 M15 M18`
- Required sections:
  - Floor-area-first inputs
  - Coverage and kit sizing
  - Different template than woodworking pages
- Internal links:
  - `/epoxy-coverage-calculator`
  - `/epoxy-cost-calculator`
  - `/how-much-epoxy-do-i-need`

### Page 11
- URL: `/void-fill-epoxy-calculator`
- Primary intent: Estimate epoxy for cracks, knots, voids, and small fills
- Primary keyword cluster: `void fill epoxy calculator`
- Supporting variants: `epoxy void filling calculator`, `crack fill epoxy calculator`
- Title: `Void Fill Epoxy Calculator for Cracks & Knots`
- H1: `Void Fill Epoxy Calculator`
- Meta description: `Calculate epoxy for cracks, knots, and void fills with small-volume estimates, waste buffer, and unit conversion.`
- Modules: `M01 M02 M03 M05 M06 M08 M09 M10 M11 M12 M13 M18`
- Required sections:
  - Small-volume fill calculator
  - Irregular-shape guidance
  - Ounces and liters emphasis
- Internal links:
  - `/epoxy-volume-calculator`
  - `/epoxy-unit-converter`
  - `/epoxy-waste-factor-guide`

### Page 12
- URL: `/round-epoxy-table-calculator`
- Primary intent: Estimate round table or round mold epoxy needs
- Primary keyword cluster: `round epoxy table calculator`
- Supporting variants: `round table epoxy calculator`, `round resin table calculator`
- Title: `Round Epoxy Table Calculator`
- H1: `Round Epoxy Table Calculator`
- Meta description: `Calculate epoxy resin for round tables and circular molds with diameter-based volume, waste, and project planning guidance.`
- Modules: `M01 M02 M03 M05 M06 M09 M10 M11 M12 M13 M18`
- Required sections:
  - Diameter-based calculator
  - Round formula summary
  - Related shape guidance
- Internal links:
  - `/epoxy-volume-calculator`
  - `/table-top-epoxy-calculator`
  - `/epoxy-unit-converter`

## 4.3 Guide / Comparison / Reference Pages

### Page 13
- URL: `/how-much-epoxy-do-i-need`
- Primary intent: Answer broad quantity question and drive users to the right calculator
- Primary keyword cluster: `how much epoxy do i need`
- Supporting variants: `how much resin do i need epoxy`, `how to calculate epoxy needed`
- Title: `How Much Epoxy Do I Need? Formula, Chart & Calculator`
- H1: `How Much Epoxy Do I Need?`
- Meta description: `Learn how to calculate epoxy needs by volume, coverage, thickness, and waste, then use the right calculator for your project.`
- Modules: `M01 M16 M13 M15 M17`
- Required sections:
  - Direct answer
  - Formula summary
  - Which calculator to use by project type
  - Quick reference table
- Internal links:
  - `/epoxy-calculator`
  - `/epoxy-coverage-calculator`
  - `/epoxy-volume-calculator`
  - `/epoxy-unit-converter`

### Page 14
- URL: `/how-much-epoxy-do-i-need-for-a-river-table`
- Primary intent: Answer river-table-specific quantity question
- Primary keyword cluster: `how much epoxy do i need for a river table`
- Supporting variants: `how much resin for river table`, `river table epoxy amount`
- Title: `How Much Epoxy for a River Table? Calculator & Guide`
- H1: `How Much Epoxy Do You Need for a River Table?`
- Meta description: `Estimate how much epoxy a river table needs with measurement tips, waste guidance, segment-based planning, and a dedicated calculator.`
- Modules: `M01 M16 M08 M13 M17 M19`
- Required sections:
  - Direct answer
  - Measurement pitfalls
  - Segment-vs-average explanation
  - Embedded river table CTA
- Internal links:
  - `/river-table-epoxy-calculator`
  - `/how-to-measure-a-river-table-for-epoxy`
  - `/deep-pour-epoxy-calculator`
  - `/epoxy-cost-calculator`

### Page 15
- URL: `/how-to-measure-a-river-table-for-epoxy`
- Primary intent: Teach measurement method for irregular river shapes
- Primary keyword cluster: `how to measure a river table for epoxy`
- Supporting variants: `measure river table for resin`, `river width measurement for epoxy`
- Title: `How to Measure a River Table for Epoxy`
- H1: `How to Measure a River Table for Epoxy`
- Meta description: `Learn how to measure a river table for epoxy using segment widths, average depth, waste allowance, and practical accuracy tips.`
- Modules: `M01 M16 M08 M09 M13 M17 M19`
- Required sections:
  - Step-by-step measurement method
  - Segment example
  - Common mistakes
  - Calculator CTA
- Internal links:
  - `/river-table-epoxy-calculator`
  - `/how-much-epoxy-do-i-need-for-a-river-table`
  - `/epoxy-waste-factor-guide`

### Page 16
- URL: `/deep-pour-vs-table-top-epoxy`
- Primary intent: Compare resin types and help users choose the correct one
- Primary keyword cluster: `deep pour vs table top epoxy`
- Supporting variants: `deep pour or tabletop epoxy`, `what epoxy for river table`
- Title: `Deep Pour vs Table Top Epoxy: Which Should You Use?`
- H1: `Deep Pour vs Table Top Epoxy`
- Meta description: `Compare deep pour and table top epoxy by thickness, cure behavior, use case, and project fit for river tables, slabs, and coatings.`
- Modules: `M01 M16 M07 M09 M13 M17`
- Required sections:
  - Comparison table
  - Use-case recommendations
  - Common decision mistakes
- Internal links:
  - `/deep-pour-epoxy-calculator`
  - `/table-top-epoxy-calculator`
  - `/river-table-epoxy-calculator`

### Page 17
- URL: `/epoxy-waste-factor-guide`
- Primary intent: Explain overage, waste, and extra-buy logic
- Primary keyword cluster: `epoxy waste factor`
- Supporting variants: `how much extra epoxy should i buy`, `epoxy overage guide`
- Title: `Epoxy Waste Factor Guide: How Much Extra to Buy`
- H1: `Epoxy Waste Factor Guide`
- Meta description: `Learn how much extra epoxy to buy for waste, seepage, edge soak-in, mixing loss, and irregular project geometry.`
- Modules: `M01 M16 M13 M15 M17 M20`
- Required sections:
  - Waste sources
  - Suggested ranges
  - When to use higher buffers
- Internal links:
  - `/epoxy-calculator`
  - `/river-table-epoxy-calculator`
  - `/void-fill-epoxy-calculator`
  - `/epoxy-cost-calculator`

### Page 18
- URL: `/epoxy-coverage-chart`
- Primary intent: Provide fast reference tables for coverage
- Primary keyword cluster: `epoxy coverage chart`
- Supporting variants: `epoxy coverage table`, `epoxy coverage reference`
- Title: `Epoxy Coverage Chart: Sq Ft, Thickness & Volume`
- H1: `Epoxy Coverage Chart`
- Meta description: `Use this epoxy coverage chart to estimate resin by square footage, thickness, and volume, then move to a detailed calculator.`
- Modules: `M01 M16 M15 M17`
- Required sections:
  - Quick coverage tables
  - Thickness examples
  - Calculator CTA
- Internal links:
  - `/epoxy-coverage-calculator`
  - `/table-top-epoxy-calculator`
  - `/countertop-epoxy-calculator`
  - `/garage-floor-epoxy-calculator`

### Page 19
- URL: `/epoxy-mixing-ratio-guide`
- Primary intent: Explain mix ratios and part A/B planning
- Primary keyword cluster: `epoxy mixing ratio guide`
- Supporting variants: `part a part b epoxy calculator`, `epoxy mix ratio chart`
- Title: `Epoxy Mixing Ratio Guide: Part A / Part B Calculator`
- H1: `Epoxy Mixing Ratio Guide`
- Meta description: `Understand epoxy mix ratios, part A/B calculations, and practical batch planning for river tables, void fills, and coating jobs.`
- Modules: `M01 M16 M13 M15 M17`
- Required sections:
  - Ratio explanation
  - Part A/B examples
  - Mini calculation helper
- Internal links:
  - `/epoxy-calculator`
  - `/deep-pour-epoxy-calculator`
  - `/epoxy-cost-calculator`

### Page 20
- URL: `/epoxy-cost-calculator`
- Primary intent: Estimate material cost
- Primary keyword cluster: `epoxy cost calculator`
- Supporting variants: `how much does epoxy cost for a river table`, `epoxy project cost calculator`
- Title: `Epoxy Cost Calculator for River Tables & Coatings`
- H1: `Epoxy Cost Calculator`
- Meta description: `Estimate epoxy project cost by resin volume, kit size, waste, and price input for river tables, coatings, and deep pours.`
- Modules: `M01 M02 M05 M06 M14 M17 M18`
- Required sections:
  - Price inputs
  - Cost summary
  - Waste cost explanation
  - Related calculators
- Internal links:
  - `/epoxy-calculator`
  - `/river-table-epoxy-calculator`
  - `/deep-pour-epoxy-calculator`
  - `/epoxy-waste-factor-guide`

## 4.4 Converter Hub

### Page 21
- URL: `/epoxy-unit-converter`
- Primary intent: Convert project units and support epoxy planning
- Primary keyword cluster: `epoxy unit converter`
- Supporting variants: `cubic inches to gallons epoxy`, `liters to gallons resin calculator`, `ounces to gallons epoxy`
- Title: `Epoxy Unit Converter: Inches, Gallons, Liters & Ounces`
- H1: `Epoxy Unit Converter`
- Meta description: `Convert cubic inches, gallons, liters, quarts, and ounces for epoxy projects with quick formulas, examples, and related calculators.`
- Modules: `M01 M02 M03 M13 M15 M17`
- Required sections:
  - Multi-unit converter
  - Formula summary
  - Quick reference conversions
  - Example project conversions
- Internal links:
  - `/epoxy-calculator`
  - `/epoxy-volume-calculator`
  - `/void-fill-epoxy-calculator`
  - `/round-epoxy-table-calculator`

## 5. Trust / Site Quality Pages

### Page 22
- URL: `/methodology`
- Title: `Epoxy Calculator Methodology`
- H1: `How Our Epoxy Calculations Work`
- Required sections:
  - Formula sources
  - Conversion constants
  - Waste logic
  - Estimate disclaimer
  - When users should verify with product documentation

### Page 23
- URL: `/about`
- Title: `About Epoxy Project Planner`
- H1: `About This Epoxy Planning Tool`
- Required sections:
  - Why the site exists
  - What makes it different
  - Audience

### Page 24
- URL: `/authors`
- Title: `Authors and Editorial Standards`
- H1: `Authors and Editorial Standards`
- Required sections:
  - Author profiles
  - Expertise notes
  - Update process

### Page 25
- URL: `/contact`
- Title: `Contact`
- H1: `Contact`
- Required sections:
  - Contact form or email
  - Feedback path for formula corrections

### Page 26
- URL: `/faq`
- Title: `Epoxy Calculator FAQ`
- H1: `Epoxy Calculator FAQ`
- Required sections:
  - Top site-wide questions
  - Links to specific calculators and guides

## 6. Internal Linking Rules

### 6.1 Every indexable page must
- [ ] Link to at least 3 relevant indexable pages
- [ ] Link upward to its hub or parent intent
- [ ] Link sideways to 2-4 adjacent relevant tools/guides
- [ ] Link downward to the most specific calculator when appropriate

### 6.2 Head-term pages should link to
- [ ] Scenario calculators
- [ ] Converter
- [ ] Cost page
- [ ] Core guides

### 6.3 Scenario pages should link to
- [ ] Their closest guide page
- [ ] Cost calculator
- [ ] Product comparison page if relevant
- [ ] At least one broader hub

### 6.4 Guide pages should link to
- [ ] The calculator that solves the task
- [ ] The closest adjacent guide
- [ ] A broader hub page

## 7. Noindex / Canonical Rules

- [ ] Query parameter states use canonical to the base page
- [ ] Saved calculation variants are not indexable by default
- [ ] Filtered or experimental states are `noindex`
- [ ] Canonical URLs always point to the final clean page URL

## 8. AdSense / Affiliate Placement Rules

- [ ] Do not place ads above the primary calculator input
- [ ] Do not interrupt calculation flow with ads
- [ ] Show affiliate CTA only after result and explanation
- [ ] Keep ad density lower on calculator-heavy sections
- [ ] Use neutral affiliate CTA copy by default

## 9. Launch Checklist

- [ ] All 26 pages built
- [ ] All titles and metas implemented
- [ ] All H1s unique
- [ ] All internal links live
- [ ] All breadcrumbs live
- [ ] All calculators tested with sample values
- [ ] Mobile layout tested on core breakpoints
- [ ] Sitemap index generated
- [ ] `robots.txt` live
- [ ] Canonical tags verified
- [ ] Search Console ready
- [ ] Analytics events verified

## 10. Recommended Build Order

This is not a product phase plan. It is the fastest engineering order for one-pass implementation.

1. Shared layout, nav, footer, breadcrumb, SEO helpers
2. Shared calculator shell and result modules
3. Head-term pages
4. River table and deep pour pages
5. Remaining scenario pages
6. Guide pages
7. Converter page
8. Trust pages
9. Sitemap, robots, schema, noindex/canonical rules
10. Analytics and final QA
