## 2025-06-11 - Accessibility First
**Learning:** In an empty repository, the most impactful UX contribution is establishing a solid accessibility foundation. This includes defining clear focus indicators and semantic landmarks that prevent future accessibility debt.
**Action:** Always start UI development with a "Skip to Content" link and visible focus styles to set the standard for the rest of the project.

## 2026-06-13 - Semantic Landmarks and Navigation
**Learning:** Establishing semantic landmarks like `<header>` and `<footer>` early ensures that screen reader users can navigate the structure of the site efficiently from day one. Additionally, including core documents like the Security Policy in the footer improves transparency and trust.
**Action:** Always wrap top-level content in appropriate semantic landmarks to provide clear navigation paths for assistive technologies.

## 2026-06-29 - Theme-Aware Selection Colors
**Learning:** Standard text selection colors can feel disconnected from a brand's identity, especially when switching between light and dark modes. Implementing theme-aware ::selection styles using CSS variables ensures a cohesive and high-contrast experience that respects the user's preferred color scheme while reinforcing brand consistency.
**Action:** Use CSS variables for ::selection background and text colors to maintain brand harmony and ensure accessibility (contrast) across different themes.
