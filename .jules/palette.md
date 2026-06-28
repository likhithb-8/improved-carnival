## 2025-06-11 - Accessibility First
**Learning:** In an empty repository, the most impactful UX contribution is establishing a solid accessibility foundation. This includes defining clear focus indicators and semantic landmarks that prevent future accessibility debt.
**Action:** Always start UI development with a "Skip to Content" link and visible focus styles to set the standard for the rest of the project.

## 2026-06-13 - Semantic Landmarks and Navigation
**Learning:** Establishing semantic landmarks like `<header>` and `<footer>` early ensures that screen reader users can navigate the structure of the site efficiently from day one. Additionally, including core documents like the Security Policy in the footer improves transparency and trust.
**Action:** Always wrap top-level content in appropriate semantic landmarks to provide clear navigation paths for assistive technologies.

## 2026-06-24 - Theme-Aware Selection and Contrast
**Learning:** Hardcoded accessibility colors (like `white` text on skip-links) can fail contrast requirements when a project supports dark mode. Using theme-aware CSS variables for both selection backgrounds and accessibility components ensures a consistent, high-contrast experience across all color schemes.
**Action:** Define `--selection-bg` and `--selection-text` variables that adapt to the theme, and use them for any high-visibility UI components to guarantee accessibility.
