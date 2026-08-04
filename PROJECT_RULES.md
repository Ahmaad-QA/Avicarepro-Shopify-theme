# AVICARE PRO Project Rules

## Purpose
This document defines the working rules for all future Shopify development work on the AVICARE PRO theme.

## Core principles
- Build for a premium veterinary brand with a scientific, trustworthy, high-conversion experience.
- Prioritize mobile-first layouts and fast-loading pages.
- Support Arabic and English with RTL as a mandatory requirement.
- Keep all storefront copy editable through Shopify theme settings, metafields, and translations where possible.
- Reuse existing sections, blocks, and snippets before introducing new components.
- Avoid duplicate CSS and keep styling modular.
- Preserve performance, accessibility, and maintainability.

## Shopify OS 2.0 requirements
- Use sections and blocks as the primary composition model.
- Prefer JSON templates for page structure and section placement.
- Keep theme settings centralized in config settings and use translation keys where appropriate.
- Use section groups for global areas such as header and footer.
- Avoid hard-coding section content when a settings-driven approach is possible.

## Mobile-first rule
- Design for small screens first.
- Ensure all layouts, spacing, and interactions work properly on mobile before scaling up.
- Optimize touch targets, stacking, and content hierarchy for mobile commerce.

## RTL Arabic requirement
- All new interfaces must support Arabic RTL layouts.
- Use logical CSS properties where possible instead of left/right-specific rules.
- Ensure navigation, forms, alignment, icons, and content ordering work correctly in RTL.
- Test with Arabic locale preview and verify visual directionality.

## Content and localization
- Do not hardcode visible brand text, product copy, or marketing copy directly in Liquid or CSS.
- Use Shopify schema settings, translation files, and dynamic content where appropriate.
- Keep all editable text available for localization and future content updates.

## Component reuse
- Reuse existing snippets and section patterns before creating new ones.
- Prefer extending existing reusable components rather than creating parallel implementations.
- Keep component responsibilities focused and predictable.

## CSS and styling rules
- Avoid duplicate selectors and repeated utility patterns.
- Prefer token-based color, spacing, and typography rules.
- Keep styles scoped to the section or component where possible.
- Do not introduce conflicting CSS architectures.
- Use the AVICARE PRO approved palette, spacing tokens, and component standards from the design system documentation.
- Keep new styling aligned to the existing Atelier variables and layout utilities.

## Design system rules
- All new components should follow the AVICARE PRO design system documented in docs/design-system.md.
- Do not introduce ad-hoc colors, spacing values, or typography scales that are not part of the approved system.
- Maintain consistency across buttons, cards, product cards, and editorial sections.
- Preserve premium, scientific, and trustworthy visual language across the entire storefront.

## Performance rules
- Keep JavaScript efficient and defer non-critical behavior.
- Avoid unnecessary DOM manipulation and large script bundles.
- Optimize images and media usage for mobile and global markets.
- Preserve fast initial render and smooth interaction states.

## Accessibility rules
- Maintain semantic HTML structure.
- Ensure keyboard navigation, visible focus states, and screen-reader compatibility.
- Use adequate contrast and descriptive link/button text.
- Support reduced-motion preferences where applicable.

## Liquid coding standards
- Write readable, maintainable Liquid.
- Keep logic simple and avoid deeply nested conditions where possible.
- Favor clear variable names and comments for non-obvious logic.
- Do not introduce fragile inline logic that is hard to maintain.

## Modification policy
- Do not modify existing core theme files unnecessarily.
- Keep changes scoped to the specific feature or customization being delivered.
- Preserve the integrity of the base Atelier structure unless a documented improvement is required.
