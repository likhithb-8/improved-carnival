## 2025-06-12 - Hardware-Accelerated Transitions
**Learning:** Properties that trigger the "Layout" and "Paint" stages of the browser rendering pipeline (like `top`, `left`, `margin`, `height`) are significantly more expensive to animate than "Composite-only" properties like `transform` and `opacity`. Offloading these to the GPU via `transform` ensures smoother 60fps transitions and reduces main-thread load.
**Action:** Always prefer `transform` and `opacity` for animations and transitions. Use `will-change` judiciously; for infrequently used elements like "Skip to Content" links, it can be a performance anti-pattern due to unnecessary memory allocation.

## 2025-06-14 - Prioritizing the Critical Path
**Learning:** Browsers have a default priority for different resource types. Critical CSS is high priority by default, but in complex pages, other resources can compete for bandwidth. Explicitly setting `fetchpriority="high"` on critical stylesheets ensures they are fetched as early as possible, directly improving First Contentful Paint (FCP).
**Action:** Use `fetchpriority="high"` for critical-path resources like main stylesheets or hero images to ensure the fastest possible initial render.

## 2026-06-13 - Perceived Performance and Color Schemes
**Learning:** Using the `<meta name="color-scheme" content="light dark">` tag allows the browser to immediately render the initial canvas in the user's preferred theme, even before CSS is parsed. This eliminates the "Flash of Unstyled Content" (FOUC) for dark-mode users, significantly improving perceived performance.
**Action:** Always include the color-scheme meta tag in the HTML head when supporting multiple themes to ensure a seamless initial render.
