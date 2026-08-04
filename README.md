# AVICARE PRO Shopify Theme

AVICARE PRO is a premium Shopify OS 2.0 ecommerce theme built on top of the Atelier foundation. It is being customized for the AVICARE PRO veterinary pigeon supplement brand with a modular, scalable, and production-ready approach.

## Project Overview

This project is a premium Shopify theme tailored for the AVICARE PRO brand. The theme is designed to support a high-conversion ecommerce experience for a veterinary-focused pigeon supplement business while maintaining a scientific, premium, and trustworthy brand presence.

The implementation follows a modular Shopify OS 2.0 architecture and is being developed incrementally through structured stories and documented milestones.

## Tech Stack

- Shopify OS 2.0
- Liquid
- HTML
- CSS
- JavaScript
- Git
- GitHub
- Shopify CLI
- Theme Check

## Project Structure

The theme is organized into the following core directories:

- assets/ for shared styles, scripts, and theme assets
- blocks/ for reusable content blocks
- config/ for theme settings and schema
- docs/ for project documentation and planning
- layout/ for the main page shell
- locales/ for translations and localization content
- sections/ for modular page sections
- snippets/ for reusable Liquid components
- templates/ for page templates and JSON structure

## Documentation

Key project documentation includes:

- PROJECT_RULES.md — development rules and standards for the project
- DEVELOPMENT_PLAN.md — phased roadmap for implementation
- BRAND_GUIDE.md — brand identity and visual direction
- TECH_STACK.md — technical stack overview
- docs/design-system.md — AVICARE PRO design system guidance
- docs/component-architecture.md — reusable component planning
- docs/testing.md — QA checklist and verification guidance
- docs/architecture.md — theme architecture overview

## Development Workflow

The project is developed one story at a time.

1. Pick one Story
2. Implement only that Story
3. Run Theme Check
4. Test with Shopify Theme Dev
5. Commit the change
6. Push to GitHub

No Story should include unrelated work.

## Local Development

Use the following commands during development:

```bash
shopify theme dev
shopify theme check
git status
git add .
git commit -m "Story X"
git push
```

## Development Principles

This project is built with the following principles in mind:

- Extends Atelier rather than replacing it
- Avoids editing core architecture when possible
- Uses reusable Sections and Snippets
- Uses design tokens instead of hardcoded values
- Supports RTL for Arabic and English content
- Prioritizes performance and maintainability

## Current Status

- [x] Git initialized
- [x] GitHub connected
- [x] Theme Check passing
- [x] Story 1.1 completed

- [ ] Header
- [ ] Homepage
- [ ] Product Page
- [ ] Collections
- [ ] Footer
- [ ] Performance

## License

This is a private commercial project for AVICARE PRO.
