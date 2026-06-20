## 2025-06-12 - Hardware-Accelerated Transitions
**Learning:** Properties that trigger the "Layout" and "Paint" stages of the browser rendering pipeline (like `top`, `left`, `margin`, `height`) are significantly more expensive to animate than "Composite-only" properties like `transform` and `opacity`. Offloading these to the GPU via `transform` ensures smoother 60fps transitions and reduces main-thread load.
**Action:** Always prefer `transform` and `opacity` for animations and transitions. Use `will-change` judiciously; for infrequently used elements like "Skip to Content" links, it can be a performance anti-pattern due to unnecessary memory allocation.

## 2026-06-13 - Perceived Performance and Color Schemes
**Learning:** Using the `<meta name="color-scheme" content="light dark">` tag allows the browser to immediately render the initial canvas in the user's preferred theme, even before CSS is parsed. This eliminates the "Flash of Unstyled Content" (FOUC) for dark-mode users, significantly improving perceived performance.
**Action:** Always include the color-scheme meta tag in the HTML head when supporting multiple themes to ensure a seamless initial render.

## 2026-06-20 - Optimized Rendering with content-visibility
**Learning:** Using `content-visibility: auto` along with `contain-intrinsic-size` allows the browser to skip the rendering work (layout and painting) for off-screen elements. This is more efficient than `contain: content` or `contain: layout` alone as it completely bypasses the rendering lifecycle for the element until it approaches the viewport.
**Action:** Apply `content-visibility: auto` to large, non-critical landmarks like footers to improve initial load and scroll performance.
