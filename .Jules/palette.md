## 2025-05-24 - [Dark Mode Interactive Elements]
**Learning:** When implementing dark mode, standard background colors for interactive elements (like #1a1a1a) may conflict with the dark mode body background. This can render buttons invisible.
**Action:** In dark mode, invert or adjust interactive element colors (e.g., using brand orange #ff9800) to ensure they remain distinct and accessible.

## 2026-05-26 - [Global Selection Styles and Visibility]
**Learning:** Global `::selection` styles using brand colors can cause visibility issues when applied to elements that already use those brand colors as a background (e.g., headers).
**Action:** Always provide specific `::selection` overrides for components with background colors that match the global selection style to ensure text remains readable when selected.

## 2026-06-05 - [Component-Specific Selection Contrast in Dark Mode]
**Learning:** Global selection styles using brand colors can create "invisible" selections when applied to interactive elements that use the same brand color as a background. This is especially prevalent in Dark Mode where CTA colors are often inverted to the primary brand color.
**Action:** Implement specific `::selection` and `*::selection` overrides for brand-colored components to ensure sufficient contrast (e.g., inverting to a dark background with light text).

## 2026-06-07 - [Reduced Motion Accessibility Support]
**Learning:** Global `prefers-reduced-motion` support is critical for users with vestibular disorders. A robust implementation requires forcing `scroll-behavior: auto` and zeroing out animation/transition durations via `!important` to ensure user settings are respected across all components.
**Action:** Always implement a global `@media (prefers-reduced-motion: reduce)` block that resets animations, transitions, and scroll behavior to ensure accessibility compliance.

## 2026-06-08 - [Delightful CTA Micro-Interactions]
**Learning:** Combining a subtle vertical lift (`translateY(-2px)`) with an elastic icon transformation (`scale(1.15)` and `rotate(12deg)`) using a `cubic-bezier(0.34, 1.56, 0.64, 1)` easing creates a high-quality, tactile feedback loop that makes the primary action feel more responsive and delightful.
**Action:** Use elastic easing for icon transitions to provide a polished 'bounce' effect that rewards user interaction.
