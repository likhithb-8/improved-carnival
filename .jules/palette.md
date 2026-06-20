## 2025-06-11 - Accessibility First
**Learning:** In an empty repository, the most impactful UX contribution is establishing a solid accessibility foundation. This includes defining clear focus indicators and semantic landmarks that prevent future accessibility debt.
**Action:** Always start UI development with a "Skip to Content" link and visible focus styles to set the standard for the rest of the project.

## 2026-06-13 - Semantic Landmarks and Navigation
**Learning:** Establishing semantic landmarks like `<header>` and `<footer>` early ensures that screen reader users can navigate the structure of the site efficiently from day one. Additionally, including core documents like the Security Policy in the footer improves transparency and trust.
**Action:** Always wrap top-level content in appropriate semantic landmarks to provide clear navigation paths for assistive technologies.

## 2026-06-20 - Semantic Footer Navigation
**Learning:** Using pipe-separated links in footers is an accessibility anti-pattern because screen readers may announce the pipe character, and it lacks the structural context of a navigation list. Refactoring to a semantic `<nav>` with an unordered list provides clear boundaries and improves discoverability for assistive technology users.
**Action:** Always prefer semantic list-based navigation (`<ul>` within `<nav>`) for footer links to ensure a robust and accessible navigation experience.
