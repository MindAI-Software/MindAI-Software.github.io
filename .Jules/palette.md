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
