## 2025-06-11 - Accessibility First
**Learning:** In an empty repository, the most impactful UX contribution is establishing a solid accessibility foundation. This includes defining clear focus indicators and semantic landmarks that prevent future accessibility debt.
**Action:** Always start UI development with a "Skip to Content" link and visible focus styles to set the standard for the rest of the project.

## 2026-06-13 - Semantic Landmarks and Navigation
**Learning:** Establishing semantic landmarks like `<header>` and `<footer>` early ensures that screen reader users can navigate the structure of the site efficiently from day one. Additionally, including core documents like the Security Policy in the footer improves transparency and trust.
**Action:** Always wrap top-level content in appropriate semantic landmarks to provide clear navigation paths for assistive technologies.

## 2026-07-20 - Custom Selection Color Overrides
**Learning:** Browsers defaults for selection styling can sometimes result in low contrast or break visual cohesiveness. Implementing tailored `::selection` styles that respect the current color-scheme (light/dark mode) guarantees both high contrast (WCAG standards) and brand-consistent visual delight.
**Action:** Always define high-contrast theme-specific colors for `::selection` in styles.css.
