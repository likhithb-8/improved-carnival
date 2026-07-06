## 2025-06-11 - Accessibility First
**Learning:** In an empty repository, the most impactful UX contribution is establishing a solid accessibility foundation. This includes defining clear focus indicators and semantic landmarks that prevent future accessibility debt.
**Action:** Always start UI development with a "Skip to Content" link and visible focus styles to set the standard for the rest of the project.

## 2026-06-13 - Semantic Landmarks and Navigation
**Learning:** Establishing semantic landmarks like `<header>` and `<footer>` early ensures that screen reader users can navigate the structure of the site efficiently from day one. Additionally, including core documents like the Security Policy in the footer improves transparency and trust.
**Action:** Always wrap top-level content in appropriate semantic landmarks to provide clear navigation paths for assistive technologies.

## 2026-06-29 - Theme-Aware Selection Polish
**Learning:** Custom text selection colors are a high-impact, low-effort micro-UX touch that reinforces brand identity. By using theme-aware CSS variables, we ensure that the selection remains accessible and visually pleasing across both light and dark modes, avoiding the "default blue" look that can feel out of place in custom dark themes.
**Action:** Implement `::selection` styles using theme-aware variables to maintain brand consistency and high contrast across all supported color schemes.
