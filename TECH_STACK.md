# AVICARE PRO Technical Stack

## Core platform
- Shopify Online Store 2.0
- Shopify Liquid templating language
- JSON templates for page and section structure
- Section-based theme architecture

## Theme architecture
- Layout files define the base shell of the storefront.
- Sections provide reusable page building blocks.
- Blocks allow modular content inside sections.
- Snippets provide reusable UI fragments and logic blocks.
- Assets contain CSS, JavaScript, and theme modules.

## Liquid and templating
Liquid is used for:
- Rendering dynamic content
- Building reusable snippets and section logic
- Connecting theme settings to storefront content
- Managing localization and conditional rendering

## OS 2.0 structure
The theme uses:
- Section groups for header and footer
- JSON templates for page composition
- Settings schema for configurable theme options
- Reusable blocks and snippets for modular content creation

## CSS architecture
- Base styles are centralized in assets/base.css.
- Theme styling is supported through shared snippet-based style helpers.
- Styling should remain modular and avoid duplication.

## JavaScript architecture
- JavaScript modules are organized under assets/.
- Script loading is managed through snippets/scripts.liquid.
- Existing behavior includes interactive UI, product forms, media handling, drawer interactions, and section hydration.

## Development workflow
1. Review the existing base theme structure before editing.
2. Extend using sections, blocks, snippets, and settings rather than hard-coded markup.
3. Keep styling and logic aligned with the existing architecture.
4. Validate layout behavior across desktop, mobile, and RTL.
5. Preserve performance and accessibility standards throughout development.
