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

## 2026-06-20 - [Staggered Page Transitions]
**Learning:** Staggered entrance animations for page segments (header, main, footer) improve the perceived quality of the interface and guide the user's attention naturally from top to bottom.
**Action:** Use CSS animation delays on primary container elements to create a polished sequence during initial page load.

## 2026-06-22 - [Progressive Enhancement for Sharing]
**Learning:** Using 'navigator.share' provides a native, integrated experience on mobile, but requires a robust fallback for desktop/older browsers. Implementing a clipboard copy with immediate, localized visual feedback ('Copied!') ensures a consistent and helpful experience across all devices.
**Action:** Always provide a functional fallback (like clipboard copy) when using modern web APIs like Web Share, and include transient success indicators to confirm the action.

## 2026-06-25 - [Icon Swap for Action Confirmation]
**Learning:** Visual confirmation of an action (like copying to clipboard) is more effective when the primary interaction element (the icon) transforms into a success indicator (a checkmark). This provides immediate, focused feedback that doesn't require the user to move their eyes to a separate toast or label.
**Action:** Use an icon-wrapper with absolute positioning to smoothly swap between action and confirmation icons during transient success states.

## 2026-06-27 - [Transient State Synchronization]
**Learning:** Transient UI states (like "Copied!") can become desynchronized if multiple triggers occur within the timeout period. Managing a global timeout variable and clearing it before new interactions, while simultaneously updating ARIA labels, ensures a reliable and accessible user experience.
**Action:** Always use `clearTimeout` for temporary feedback states and synchronize them with dynamic ARIA attribute updates to prevent state-drift and improve screen reader support.

## 2026-06-30 - [Rich Link Previews for Sharing UX]
**Learning:** The "Share" interaction doesn't end with a "Copied!" message; the quality of the resulting link preview (Open Graph/Twitter Cards) is a critical part of the user's social experience with the brand.
**Action:** Always synchronize sharing functionality with proper meta tag implementation to ensure rich, informative link previews across all platforms.
