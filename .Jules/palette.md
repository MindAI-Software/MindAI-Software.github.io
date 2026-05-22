## 2025-03-18 - [Repository Bootstrapping UX]
**Learning:** Empty repositories intended for GitHub Pages create a poor user experience. Bootstrapping a simple, accessible landing page provides immediate value.
**Action:** Prioritize creating a semantic `index.html` for new GitHub Pages repos.

## 2025-03-18 - [Color Contrast for Accessibility]
**Learning:** Using white text on an orange background (#ff9800) often results in poor contrast (approx. 2.27:1), failing WCAG AA standards. Switching to dark text (#1a1a1a) significantly improves readability.
**Action:** Always check color contrast for branding colors, especially with white text on bright backgrounds.

## 2025-03-18 - [Scope Management in Micro-UX]
**Learning:** For empty repositories, providing a basic landing page is high UX value, but must be balanced against "micro-UX" constraints. Keeping implementation extremely lean (under 40 lines) helps maintain focus on the "micro" aspect while delivering "macro" value.
**Action:** Always strive for maximal UX impact with minimal code footprint; favor semantic HTML and CSS over additional tooling (like dummy package.json) for static projects.

## 2025-05-20 - [Thematic Continuity and Mobile UX]
**Learning:** Synchronizing the app's theme with the browser UI via `<meta name="theme-color">` and supporting `prefers-color-scheme` creates a more immersive and accessible experience, especially on mobile devices.
**Action:** Always include theme-color metadata and Dark Mode styles to respect user system preferences and enhance the "platform-native" feel of web apps.

## 2025-05-22 - [Keyboard Navigation with Skip Links]
**Learning:** For minimalist static sites, a "Skip to Content" link is a high-impact, low-effort accessibility win. It's often overlooked in small projects but essential for keyboard-only users to bypass repetitive header content.
**Action:** Always include a skip-to-content link in the boilerplate for new web projects to ensure immediate WCAG compliance for navigation.
