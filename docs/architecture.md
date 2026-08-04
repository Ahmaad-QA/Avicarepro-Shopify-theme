# Theme Architecture

## Overview
The AVICARE PRO theme is based on Shopify's Atelier theme and follows a modern Online Store 2.0 structure. The architecture is section-driven, with reusable snippets, blocks, and shared assets supporting a scalable storefront.

## Core directories
- assets/: shared CSS, JavaScript, and theme modules
- blocks/: reusable content blocks that can be inserted into sections
- config/: settings schema and theme config data
- layout/: base page shell, including theme.liquid
- locales/: translation and schema files for internationalization
- sections/: page sections for content and layout composition
- snippets/: reusable UI fragments and logic helpers
- templates/: JSON templates controlling page structure

## How the theme is organized
- Layout files provide the overall page shell.
- Sections define the modular content areas of the store.
- Blocks enable flexible content composition inside sections.
- Snippets encapsulate smaller reusable UI elements and shared logic.
- Assets hold global styling and behavior that can be leveraged across the theme.

## Recommended approach for customization
Future work should extend the current architecture rather than replacing it. Prefer adding or adapting sections and snippets over introducing isolated custom templates or duplicated UI patterns.
