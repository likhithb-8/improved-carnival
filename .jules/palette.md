## 2025-06-11 - Accessibility First
**Learning:** In an empty repository, the most impactful UX contribution is establishing a solid accessibility foundation. This includes defining clear focus indicators and semantic landmarks that prevent future accessibility debt.
**Action:** Always start UI development with a "Skip to Content" link and visible focus styles to set the standard for the rest of the project.

## 2026-06-13 - Semantic Landmarks and Navigation
**Learning:** Establishing semantic landmarks like `<header>` and `<footer>` early ensures that screen reader users can navigate the structure of the site efficiently from day one. Additionally, including core documents like the Security Policy in the footer improves transparency and trust.
**Action:** Always wrap top-level content in appropriate semantic landmarks to provide clear navigation paths for assistive technologies.

## 2026-07-14 - Skip Link Reliability and Selection Branding
**Learning:** For "Skip to Content" links to work reliably across all browsers, the target element must have `tabindex="-1"`. To prevent a jarring focus ring around the entire main content after skip-link activation, `outline: none` should be applied specifically to the target's focus state. Additionally, theme-aware `::selection` colors enhance brand identity and provide a polished micro-interaction.
**Action:** Always pair skip-link targets with `tabindex="-1"` and `outline: none`, and implement branded selection colors for both light and dark modes.
