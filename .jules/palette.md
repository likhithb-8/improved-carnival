## 2025-06-11 - Accessibility First
**Learning:** In an empty repository, the most impactful UX contribution is establishing a solid accessibility foundation. This includes defining clear focus indicators and semantic landmarks that prevent future accessibility debt.
**Action:** Always start UI development with a "Skip to Content" link and visible focus styles to set the standard for the rest of the project.

## 2026-06-13 - Semantic Landmarks and Navigation
**Learning:** Establishing semantic landmarks like `<header>` and `<footer>` early ensures that screen reader users can navigate the structure of the site efficiently from day one. Additionally, including core documents like the Security Policy in the footer improves transparency and trust.
**Action:** Always wrap top-level content in appropriate semantic landmarks to provide clear navigation paths for assistive technologies.

## 2026-06-29 - Brand-Aligned Selection Colors
**Learning:** Customizing the `::selection` pseudo-element with brand-aware, theme-consistent colors enhances visual delight while reinforcing brand identity. Using high-contrast pairings (e.g., Blue 200/800 for light, Blue 800/50 for dark) ensures that the selection remains accessible across different color schemes.
**Action:** Implement theme-aware `--selection-bg` and `--selection-text` variables to maintain accessibility and brand consistency in text interactions.
