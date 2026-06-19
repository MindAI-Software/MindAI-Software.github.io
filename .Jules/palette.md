## 2025-03-18 - [Repository Bootstrapping UX]
**Learning:** Empty repositories intended for GitHub Pages create a poor user experience. Bootstrapping a simple, accessible landing page provides immediate value.
**Action:** Prioritize creating a semantic `index.html` for new GitHub Pages repos.

## 2025-03-18 - [Color Contrast for Accessibility]
**Learning:** Using white text on an orange background (#ff9800) often results in poor contrast (approx. 2.27:1), failing WCAG AA standards. Switching to dark text (#1a1a1a) significantly improves readability.
**Action:** Always check color contrast for branding colors, especially with white text on bright backgrounds.

## 2026-06-16 - [Tactile Feedback Polish]
**Learning:** High-quality micro-interactions require synchronization between the container (button) and its internal elements (SVG icons). Only scaling the container can feel "disconnected" if the icon doesn't respond similarly during the `:active` state.
**Action:** Always sync `:active` transforms between interactive containers and their internal visual indicators (like SVG icons) to provide a cohesive tactile response.

## 2026-06-18 - [Skip Link Visual Affordance]
**Learning:** "Skip to content" links are often overlooked by keyboard users if they lack visual affordance. Adding a directional icon (arrow) and synchronizing its interaction states (nudge on focus, scale on active) with the site's primary CTA patterns improves discoverability and cohesion.
**Action:** Always include a visual indicator in skip links and align their micro-interactions with the established design system.

## 2026-06-19 - [Header Branding Micro-Interactions]
**Learning:** Site branding often remains static, missing an opportunity for delight. Adding a micro-interaction to a brand emoji that triggers on both hover and keyboard focus provides a cohesive experience for all users and reinforces the brand's personality.
**Action:** Incorporate "brand delight" elements like animated emojis or icons in headers, ensuring they respond to focus states to maintain accessibility.
