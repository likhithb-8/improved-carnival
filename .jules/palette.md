## 2025-06-11 - Accessibility First
**Learning:** In an empty repository, the most impactful UX contribution is establishing a solid accessibility foundation. This includes defining clear focus indicators and semantic landmarks that prevent future accessibility debt.
**Action:** Always start UI development with a "Skip to Content" link and visible focus styles to set the standard for the rest of the project.

## 2026-06-13 - Semantic Landmarks and Navigation
**Learning:** Establishing semantic landmarks like `<header>` and `<footer>` early ensures that screen reader users can navigate the structure of the site efficiently from day one. Additionally, including core documents like the Security Policy in the footer improves transparency and trust.
**Action:** Always wrap top-level content in appropriate semantic landmarks to provide clear navigation paths for assistive technologies.

## 2026-06-29 - Brand Consistency and Accessible Navigation
**Learning:** Default browser selection colors often clash with brand identity and may have poor contrast in dark mode. Implementing theme-aware selection colors ensures a cohesive experience. Additionally, subtle font-weight adjustments to skip-links significantly improve their legibility when they appear, without cluttering the layout.
**Action:** Use CSS variables for selection colors and define them for both themes. Always ensure critical accessibility tools like skip-links have high legibility when focused.
