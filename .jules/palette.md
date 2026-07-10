## 2025-06-11 - Accessibility First
**Learning:** In an empty repository, the most impactful UX contribution is establishing a solid accessibility foundation. This includes defining clear focus indicators and semantic landmarks that prevent future accessibility debt.
**Action:** Always start UI development with a "Skip to Content" link and visible focus styles to set the standard for the rest of the project.

## 2026-06-13 - Semantic Landmarks and Navigation
**Learning:** Establishing semantic landmarks like `<header>` and `<footer>` early ensures that screen reader users can navigate the structure of the site efficiently from day one. Additionally, including core documents like the Security Policy in the footer improves transparency and trust.
**Action:** Always wrap top-level content in appropriate semantic landmarks to provide clear navigation paths for assistive technologies.

## 2026-06-29 - Robust Skip Links and Themed Highlights
**Learning:** For 'Skip to Content' links to function reliably across all browsers (including those that do not natively manage focus on fragment navigation), the target element (e.g., <main>) must include 'tabindex="-1"'. Additionally, theme-aware text selection colors (`::selection`) using CSS variables provide a low-effort, high-impact polish that reinforces brand identity in both light and dark modes.
**Action:** Always add 'tabindex="-1"' to fragment navigation targets and implement themed selection colors as part of the initial UI polish.
