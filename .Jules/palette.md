## 2025-03-18 - [Repository Bootstrapping UX]
**Learning:** Empty repositories intended for GitHub Pages create a poor user experience. Bootstrapping a simple, accessible landing page provides immediate value.
**Action:** Prioritize creating a semantic `index.html` for new GitHub Pages repos.

## 2025-03-18 - [Color Contrast for Accessibility]
**Learning:** Using white text on an orange background (#ff9800) often results in poor contrast (approx. 2.27:1), failing WCAG AA standards. Switching to dark text (#1a1a1a) significantly improves readability.
**Action:** Always check color contrast for branding colors, especially with white text on bright backgrounds.

## 2025-05-24 - [Dark Mode Interactive Elements]
**Learning:** When implementing dark mode, standard background colors for interactive elements (like #1a1a1a) may conflict with the dark mode body background. This can render buttons invisible.
**Action:** In dark mode, invert or adjust interactive element colors (e.g., using brand orange #ff9800) to ensure they remain distinct and accessible.

## 2026-05-26 - [Global Selection Styles and Visibility]
**Learning:** Global `::selection` styles using brand colors can cause visibility issues when applied to elements that already use those brand colors as a background (e.g., headers).
**Action:** Always provide specific `::selection` overrides for components with background colors that match the global selection style to ensure text remains readable when selected.

## 2026-06-01 - [Label in Name (WCAG 2.5.3)]
**Learning:** For accessible interactive elements, the `aria-label` must contain the visible text of the element. This ensures that users of speech-recognition software can activate the element by speaking its visible label.
**Action:** Always ensure that `aria-label` values include the visible text string (e.g., "Explore GitHub projects" for a button showing "Explore GitHub").

## 2026-06-02 - [Interactive State Differentiation]
**Learning:** Providing distinct visual feedback for `:hover` (mouse users) and `:focus-visible` (keyboard users) improves the clarity of the interface for different input methods.
**Action:** Use different styles (e.g., background-color for hover and an outline for focus) to provide unambiguous feedback to the user.

## 2026-06-04 - [External Link A11y and Smooth Transitions]
**Learning:** Combining `target="_blank"` with an explicit "(opens in a new tab)" in the `aria-label` provides a much clearer experience for screen reader users when navigating to external resources. Additionally, `scroll-behavior: smooth` on the `:root` element significantly improves the context preservation for sighted users when using skip links.
**Action:** Always pair external link target changes with updated ARIA labels and ensure root smooth scrolling is enabled for internal navigation.

## 2026-06-05 - [Component-Specific Selection Contrast in Dark Mode]
**Learning:** Global selection styles using brand colors can create "invisible" selections when applied to interactive elements that use the same brand color as a background. This is especially prevalent in Dark Mode where CTA colors are often inverted to the primary brand color.
**Action:** Implement specific `::selection` and `*::selection` overrides for brand-colored components to ensure sufficient contrast (e.g., inverting to a dark background with light text).

## 2026-06-07 - [Reduced Motion Accessibility Support]
**Learning:** Global `prefers-reduced-motion` support is critical for users with vestibular disorders. A robust implementation requires forcing `scroll-behavior: auto` and zeroing out animation/transition durations via `!important` to ensure user settings are respected across all components.
**Action:** Always implement a global `@media (prefers-reduced-motion: reduce)` block that resets animations, transitions, and scroll behavior to ensure accessibility compliance.

## 2026-06-10 - [Dark Mode Shadow Polish]
**Learning:** In dark mode, standard black box-shadows are often invisible against dark backgrounds. Using a semi-transparent version of the brand color (e.g., rgba(255, 152, 0, 0.3) for orange) creates a subtle 'glow' that effectively communicates elevation.
**Action:** Use brand-colored semi-transparent shadows for interactive elements in dark mode to preserve visual depth.

## 2026-06-11 - [Sticky Footer for Layout Stability]
**Learning:** Implementation of a sticky footer requires 'display: flex; flex-direction: column; min-height: 100vh' on 'body', 'flex: 1' on 'main', and substituting 'footer' top margins with padding to maintain layout balance on short pages.
**Action:** Use Flexbox on the body and main elements to ensure the footer stays at the bottom of the viewport on pages with minimal content.
