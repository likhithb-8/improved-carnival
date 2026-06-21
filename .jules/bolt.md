## 2025-06-12 - Hardware-Accelerated Transitions
**Learning:** Properties that trigger the "Layout" and "Paint" stages of the browser rendering pipeline (like `top`, `left`, `margin`, `height`) are significantly more expensive to animate than "Composite-only" properties like `transform` and `opacity`. Offloading these to the GPU via `transform` ensures smoother 60fps transitions and reduces main-thread load.
**Action:** Always prefer `transform` and `opacity` for animations and transitions. Use `will-change` judiciously; for infrequently used elements like "Skip to Content" links, it can be a performance anti-pattern due to unnecessary memory allocation.

## 2026-06-13 - Perceived Performance and Color Schemes
**Learning:** Using the `<meta name="color-scheme" content="light dark">` tag allows the browser to immediately render the initial canvas in the user's preferred theme, even before CSS is parsed. This eliminates the "Flash of Unstyled Content" (FOUC) for dark-mode users, significantly improving perceived performance.
**Action:** Always include the color-scheme meta tag in the HTML head when supporting multiple themes to ensure a seamless initial render.

## 2026-06-21 - Combined Rendering Containment and Content-Visibility
**Learning:** Upgrading landmarks from `contain: layout` to `contain: content` further isolates them by also containing paint, which allows the browser to skip painting off-screen elements entirely. Combining this with `content-visibility: auto` (and a proper `contain-intrinsic-size`) on major sections like the `footer` provides a significant performance boost by deferring both layout and paint until the element is actually near the viewport.
**Action:** Use `contain: content` for layout landmarks and apply `content-visibility: auto` to non-critical, potentially off-screen landmarks to optimize initial load and scroll performance.
