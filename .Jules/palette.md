## 2025-03-18 - [Repository Bootstrapping UX]
**Learning:** Empty repositories intended for GitHub Pages create a poor user experience. Bootstrapping a simple, accessible landing page provides immediate value.
**Action:** Prioritize creating a semantic `index.html` for new GitHub Pages repos.

## 2025-03-18 - [Color Contrast for Accessibility]
**Learning:** Using white text on an orange background (#ff9800) often results in poor contrast (approx. 2.27:1), failing WCAG AA standards. Switching to dark text (#1a1a1a) significantly improves readability.
**Action:** Always check color contrast for branding colors, especially with white text on bright backgrounds.

## 2025-03-18 - [Scope Management in Micro-UX]
**Learning:** For empty repositories, providing a basic landing page is high UX value, but must be balanced against "micro-UX" constraints. Keeping implementation extremely lean (under 40 lines) helps maintain focus on the "micro" aspect while delivering "macro" value.
**Action:** Always strive for maximal UX impact with minimal code footprint; favor semantic HTML and CSS over additional tooling (like dummy package.json) for static projects.
