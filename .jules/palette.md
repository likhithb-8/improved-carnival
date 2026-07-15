## 2025-06-11 - Accessibility First
**Learning:** In an empty repository, the most impactful UX contribution is establishing a solid accessibility foundation. This includes defining clear focus indicators and semantic landmarks that prevent future accessibility debt.
**Action:** Always start UI development with a "Skip to Content" link and visible focus styles to set the standard for the rest of the project.

## 2026-06-13 - Semantic Landmarks and Navigation
**Learning:** Establishing semantic landmarks like `<header>` and `<footer>` early ensures that screen reader users can navigate the structure of the site efficiently from day one. Additionally, including core documents like the Security Policy in the footer improves transparency and trust.
**Action:** Always wrap top-level content in appropriate semantic landmarks to provide clear navigation paths for assistive technologies.

## 2026-07-15 - Reliable Skip-Link Focus
**Learning:** For 'Skip to Content' links to function reliably across all browsers, the target element (e.g., `<main id="main-content">`) must include `tabindex="-1"` to receive programmatic focus. Additionally, applying `outline: none` to the target when focused prevents a disruptive visual outline while still allowing focus to be moved for screen readers.
**Action:** Always add `tabindex="-1"` and `outline: none` to the main content target of a skip link to ensure a smooth and accessible navigation experience.
