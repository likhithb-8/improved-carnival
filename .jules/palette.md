## 2025-06-11 - Accessibility First
**Learning:** In an empty repository, the most impactful UX contribution is establishing a solid accessibility foundation. This includes defining clear focus indicators and semantic landmarks that prevent future accessibility debt.
**Action:** Always start UI development with a "Skip to Content" link and visible focus styles to set the standard for the rest of the project.

## 2026-06-13 - Semantic Landmarks and Navigation
**Learning:** Establishing semantic landmarks like `<header>` and `<footer>` early ensures that screen reader users can navigate the structure of the site efficiently from day one. Additionally, including core documents like the Security Policy in the footer improves transparency and trust.
**Action:** Always wrap top-level content in appropriate semantic landmarks to provide clear navigation paths for assistive technologies.

## 2026-06-29 - Theme-Aware Accessibility
**Learning:** Hardcoding colors like 'white' for overlay elements (e.g., skip-links) can lead to insufficient contrast when the background variable changes in dark mode. Using the inverse theme variable (e.g., `--bg-color` as text on a `--focus-ring-color` background) ensures consistent, high-contrast visibility across all color schemes.
**Action:** Use theme-aware CSS variables for both background and text of focused elements to maintain WCAG-compliant contrast ratios in both light and dark modes.
