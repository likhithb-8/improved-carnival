## 2025-06-11 - Accessibility First
**Learning:** In an empty repository, the most impactful UX contribution is establishing a solid accessibility foundation. This includes defining clear focus indicators and semantic landmarks that prevent future accessibility debt.
**Action:** Always start UI development with a "Skip to Content" link and visible focus styles to set the standard for the rest of the project.

## 2026-06-13 - Semantic Landmarks and Navigation
**Learning:** Establishing semantic landmarks like `<header>` and `<footer>` early ensures that screen reader users can navigate the structure of the site efficiently from day one. Additionally, including core documents like the Security Policy in the footer improves transparency and trust.
**Action:** Always wrap top-level content in appropriate semantic landmarks to provide clear navigation paths for assistive technologies.

## 2026-06-29 - Theme-Aware Accessibility and Visual Delight
**Learning:** Hardcoded accessibility colors (like `white` for skip-links) can fail contrast requirements in dark mode or break brand consistency. Using theme-aware CSS variables for interactive elements and custom selections ensures a cohesive and inclusive user experience across all system preferences.
**Action:** Leverage CSS variables for all UI states, including focus indicators and text selection, to maintain accessibility standards in both light and dark modes.
