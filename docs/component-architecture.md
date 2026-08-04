# AVICARE PRO Component Architecture Plan

## Overview
This document defines the reusable component architecture for AVICARE PRO on top of the existing Atelier theme. The goal is to keep the storefront modular, reusable, and aligned with Shopify OS 2.0, the existing snippet and section pattern, and the AVICARE PRO design system.

## 1. Global components

### Container
- Purpose: Define the global page width and layout constraint for all content.
- Required settings:
  - width mode: narrow, normal, wide
  - horizontal padding
  - max content width
- Where it will be used:
  - all page sections
  - hero content
  - product and collection layouts
  - editorial content blocks

### Section wrapper
- Purpose: Standardize section spacing, vertical rhythm, and background treatment.
- Required settings:
  - top padding
  - bottom padding
  - section background color
  - section width mode
  - optional divider or accent line
- Where it will be used:
  - all major content sections
  - homepage modules
  - product page content blocks
  - science and program pages

### Button component
- Purpose: Provide consistent calls to action across the storefront.
- Variants:
  - Primary
  - Secondary
  - Outline
  - Text
- Required settings:
  - label
  - link
  - style variant
  - icon support
  - full width on mobile option
- Where it will be used:
  - hero CTAs
  - product cards
  - trust modules
  - purchase and inquiry actions

### Announcement bar
- Purpose: Highlight promotions, notices, or important trust messages.
- Required settings:
  - text
  - link
  - background color
  - text color
  - visibility rules
- Where it will be used:
  - top of the storefront
  - campaign or seasonal messaging

### Header
- Purpose: Provide brand navigation, localizations, search, cart access, and mobile menu handling.
- Required settings:
  - logo
  - navigation menu
  - show search
  - show localization
  - sticky behavior
  - transparent mode option
- Where it will be used:
  - all pages globally

### Footer
- Purpose: Provide brand information, navigation, legal links, and trust content.
- Required settings:
  - columns or blocks
  - newsletter option
  - social links
  - payment icons
  - copyright text
- Where it will be used:
  - all pages globally

## 2. Ecommerce components

### Product card
- Purpose: Present products with a premium, high-conversion layout.
- Required settings:
  - product image
  - product title
  - price
  - rating or review summary
  - CTA button
  - optional badge or label
- Where it will be used:
  - featured collection sections
  - homepage product grids
  - related products
  - collection pages

### Collection card
- Purpose: Encourage browsing into product categories or thematic collections.
- Required settings:
  - collection image
  - title
  - description
  - CTA
- Where it will be used:
  - collection landing pages
  - homepage category modules

### Product benefits block
- Purpose: Communicate key product benefits in a structured and trustworthy way.
- Required settings:
  - title
  - description
  - icon or image
  - optional CTA
- Where it will be used:
  - product pages
  - marketing sections

### Ingredient card
- Purpose: Showcase ingredients, formulation elements, or functional components.
- Required settings:
  - name
  - description
  - icon or visual
- Where it will be used:
  - science content sections
  - education-based pages

### Review card
- Purpose: Highlight customer feedback, testimonials, or expert validation.
- Required settings:
  - quote or review text
  - author or source
  - rating optional
- Where it will be used:
  - product pages
  - homepage trust sections

### Trust badge
- Purpose: Communicate credibility and veterinary or performance assurance.
- Required settings:
  - label
  - icon
  - supporting text
- Where it will be used:
  - product pages
  - hero sections
  - footer trust area

### FAQ item
- Purpose: Present common questions in an expandable format.
- Required settings:
  - question
  - answer
  - optional icon
- Where it will be used:
  - product pages
  - support or science pages

### Comparison table
- Purpose: Compare products, formulations, or programs clearly.
- Required settings:
  - columns
  - row labels
  - values
  - heading
- Where it will be used:
  - product comparison pages
  - category or program pages

## 3. AVICARE-specific components

### Science section card
- Purpose: Present scientific benefits, formulation focus, or research-backed content.
- Required settings:
  - title
  - description
  - icon or illustration
  - optional CTA
- Where it will be used:
  - science page
  - educational content sections

### Breeding program card
- Purpose: Show a breeding or performance program experience in a premium, structured format.
- Required settings:
  - title
  - description
  - image or icon
  - program detail list
- Where it will be used:
  - programs page
  - educational landing pages

### Racing performance card
- Purpose: Highlight performance outcomes or racing benefits in a polished visual format.
- Required settings:
  - headline
  - supporting description
  - metrics or stat block
  - optional image
- Where it will be used:
  - performance-focused sections
  - homepage feature modules

### Recovery protocol card
- Purpose: Communicate recovery-focused treatment or care protocols.
- Required settings:
  - title
  - process steps or timeline
  - supporting copy
- Where it will be used:
  - science and recovery content sections

### Veterinary trust section
- Purpose: Reinforce credibility, veterinary expertise, and scientific standards.
- Required settings:
  - heading
  - explanatory text
  - icon or badge set
  - optional CTA
- Where it will be used:
  - product pages
  - homepage trust section
  - about or science content

### Before/after performance section
- Purpose: Showcase transformation, performance change, or comparative results visually.
- Required settings:
  - before content
  - after content
  - optional caption or note
  - visual treatment
- Where it will be used:
  - performance storytelling sections
  - marketing landing pages

## 4. Shopify implementation strategy

### Recommended implementation model

| Component | Recommended implementation | Why |
| --- | --- | --- |
| Container | CSS component | It is a layout primitive and should remain reusable in CSS rather than a standalone Liquid object. |
| Section wrapper | CSS component + section setting | It is a shared layout pattern with spacing and background behavior. |
| Button component | Snippet | It is reusable UI and benefits from a central Liquid snippet with variants. |
| Announcement bar | Section | It is a global section with independent content and settings. |
| Header | Section | It is a large, global UI area that already fits Shopify section architecture. |
| Footer | Section | It is a major site-wide region and should remain section-based. |
| Product card | Snippet | It is repeated across many contexts and should be reusable from multiple sections. |
| Collection card | Snippet | It is a repeatable card pattern for different collection contexts. |
| Product benefits block | Block or snippet | Best as a reusable block inside sections when content needs flexibility. |
| Ingredient card | Snippet | It is a repeatable content block for grids and lists. |
| Review card | Snippet | It is a reusable display unit for testimonials and reviews. |
| Trust badge | Snippet | It is a small reusable visual element. |
| FAQ item | Block | It is content-driven and benefits from repeatable block structure. |
| Comparison table | Section or snippet | Use a section when it is a larger standalone module; use a snippet when embedded in other pages. |
| Science section card | Snippet | It is a repeatable content card. |
| Breeding program card | Snippet | It is a reusable marketing card. |
| Racing performance card | Snippet | It is a reusable visual card pattern. |
| Recovery protocol card | Snippet | It is a structured content module that can be repeated. |
| Veterinary trust section | Section | It is a content-rich section with a defined layout and multiple supporting blocks. |
| Before/after performance section | Section | It is a larger visual storytelling component that benefits from dedicated section structure. |

## 5. Naming convention

### Sections
- Use the prefix avicare- for all new section files.
- Example: avicare-hero.liquid, avicare-science.liquid

### Snippets
- Use descriptive names based on component purpose.
- Example: card-product.liquid, button-primary.liquid, badge-trust.liquid

### CSS classes
- Use a clear, reusable prefix such as av-component-name.
- Example: .av-button, .av-card-product, .av-section-wrapper

### Rules
- Keep names descriptive and consistent.
- Avoid overly generic names that could conflict with existing theme classes.
- Prefer lowercase with hyphen separators.
- Use the same naming pattern across sections, snippets, and CSS classes.

## 6. Development plan update
The development plan should be updated to include a dedicated component architecture phase before header and footer implementation.
