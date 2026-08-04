# AVICARE PRO Design System

## Overview
This design system is a brand-specific extension of the existing Atelier theme foundation. It uses the current Shopify theme architecture, shared layout utilities, and CSS custom properties already present in the base theme rather than introducing a separate styling framework.

## 1. Color system

### Core palette
- Primary brand: #0F4D3A
- Luxury accent: #D4AF37
- Text: #1A1A1A
- Background: #F8F7F3

### Usage rules
- Use the primary brand color for key brand surfaces, primary calls to action, headings, and emphasis moments.
- Use the luxury accent sparingly for highlights, badges, key icons, and premium detail treatment.
- Use the text color for body copy, headings, links, and form labels.
- Use the background color as the default soft neutral surface for content sections and editorial layouts.

### Contrast rules
- Maintain a minimum contrast ratio of 4.5:1 for body text and interactive controls.
- Maintain at least 3:1 for large text and non-text UI elements.
- Avoid using the accent color for extended body text.
- Keep dark text on light backgrounds and light text on dark brand surfaces.

### Button colors
- Primary buttons: primary brand background with light text.
- Secondary buttons: light background with primary border and primary text.
- Accent buttons: luxury accent background for promotional or high-intent moments, used carefully.
- Disabled states should use reduced opacity and remain legible.

### Section backgrounds
- Default content sections should use the background color as a soft neutral base.
- Brand-led sections may use the primary color as a strong surface with light text.
- Accent-led sections should remain limited to highlights, banners, or trust points rather than full-page backgrounds.

## 2. Typography system

### Base approach
The system should build on the existing Atelier typography presets and theme settings rather than replacing them. Font families should remain configurable through the theme settings while the AVICARE PRO sizing and hierarchy stay consistent.

### Heading hierarchy
- H1
  - Desktop: 56–64px
  - Mobile: 36–44px
  - Weight: 600–700
  - Line height: 1.05–1.15
- H2
  - Desktop: 40–48px
  - Mobile: 28–34px
  - Weight: 600
  - Line height: 1.1–1.2
- H3
  - Desktop: 28–32px
  - Mobile: 22–26px
  - Weight: 600
  - Line height: 1.2–1.3
- H4
  - Desktop: 22–24px
  - Mobile: 18–20px
  - Weight: 600
  - Line height: 1.25–1.35

### Body text
- Desktop: 16–18px
- Mobile: 15–16px
- Weight: 400–500
- Line height: 1.6–1.75

### Small text
- Desktop: 13–14px
- Mobile: 12–13px
- Weight: 400–500
- Line height: 1.4–1.5

### Typography rules
- Use clear hierarchy with generous spacing between headings and body content.
- Keep body text readable and premium rather than overly condensed.
- Use uppercase sparingly and only for small labels or navigation accents.
- Preserve the existing theme’s responsive typography behavior for mobile devices.

## 3. Spacing system

### Spacing tokens
- 8px: xs
- 12px: sm
- 16px: md
- 24px: lg
- 32px: xl
- 48px: 2xl
- 72px: 3xl
- 96px: 4xl

### Section spacing
- Desktop: 80–120px vertical spacing between major sections
- Mobile: 56–72px vertical spacing between major sections

### Container width
- Default page content width: use the existing normal page-width layout
- Editorial or trust-heavy content: narrow content width for readability
- Large marketing sections: full-width layout when appropriate

### Grid gaps
- Mobile: 16px
- Tablet: 24px
- Desktop: 32px

### Mobile padding
- Horizontal padding: 16px minimum
- Vertical padding: 20px minimum for compact sections
- Larger sections should increase padding gradually for better readability

## 4. Component system

### Buttons
- Height: 44px on mobile, 48px on desktop
- Radius: 999px for primary CTAs, 999px or 12px for secondary actions depending on context
- Typography: medium weight, clear label sizing, no overly decorative styling
- Hover behavior: subtle color shift, slight elevation, and visible focus state
- Use a consistent visual weight so premium CTAs feel confident without being aggressive

### Cards
- Radius: 16–20px
- Shadow: subtle elevation, restrained and premium
- Padding: 24px on mobile, 32px on desktop
- Borders: very light or none where the background already provides separation

### Product cards
- Image ratio: 4:5 for premium product imagery
- Information hierarchy: product title first, price second, trust or benefit detail third
- Maintain strong visual spacing and avoid cluttered layouts

### Images
- Use 4:5 or 16:9 aspect ratios depending on content intent
- Apply soft border radius for a premium presentation
- Preserve consistent object-fit behavior and avoid stretching

## 5. RTL system

### Arabic support rules
- Treat RTL as a first-class requirement across all new UI work.
- Use logical CSS properties whenever possible instead of hard-coded left/right rules.
- Align text to the start edge in RTL contexts.
- Mirror icon positioning and directional UI patterns where appropriate.
- Keep spacing and padding balanced for Arabic layouts rather than relying on left/right overrides.
- Ensure navigation, forms, buttons, and cards all read naturally in Arabic.

## 6. AI development rules update
To maintain this design system, future work should follow these additional rules:
- Use the approved AVICARE PRO color palette and spacing tokens instead of introducing ad-hoc values.
- Keep new UI aligned to the existing Atelier structure and shared theme variables.
- Reuse existing components and snippets before creating new visual patterns.
- Ensure every new section is responsive, accessible, and RTL-aware from the start.
- Keep typography, spacing, and component styling consistent across the full theme.
- Do not create one-off styling solutions that bypass the shared system.
