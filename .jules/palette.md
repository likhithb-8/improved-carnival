## 2025-06-11 - Accessibility First
**Learning:** In an empty repository, the most impactful UX contribution is establishing a solid accessibility foundation. This includes defining clear focus indicators and semantic landmarks that prevent future accessibility debt.
**Action:** Always start UI development with a "Skip to Content" link and visible focus styles to set the standard for the rest of the project.

## 2026-06-13 - Semantic Landmarks and Navigation
**Learning:** Establishing semantic landmarks like `<header>` and `<footer>` early ensures that screen reader users can navigate the structure of the site efficiently from day one. Additionally, including core documents like the Security Policy in the footer improves transparency and trust.
**Action:** Always wrap top-level content in appropriate semantic landmarks to provide clear navigation paths for assistive technologies.

## 2026-07-07 - Theme-Aware Accessibility and Polish
**Learning:** Default "Skip to Content" links using primary focus colors (like light blue) often fail WCAG contrast requirements in dark mode when paired with white text. Custom text selection colors provide an easy "micro-UX" win that reinforces brand identity while ensuring readability through theme-specific color pairs.
**Action:** When implementing theme-aware UIs, always verify that interactive "utility" elements like skip-links maintain at least 4.5:1 contrast in both modes, and use global `::selection` overrides to maintain a polished, branded experience.
