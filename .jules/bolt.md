## 2025-05-12 - Hardware-Accelerated Transitions
**Learning:** Properties that trigger the "Layout" and "Paint" stages of the browser rendering pipeline (like `top`, `left`, `margin`, `height`) are significantly more expensive to animate than "Composite-only" properties like `transform` and `opacity`. Offloading these to the GPU via `transform` ensures smoother 60fps transitions and reduces main-thread load.
**Action:** Always prefer `transform` and `opacity` for animations and transitions. Use `will-change` judiciously; for infrequently used elements like "Skip to Content" links, it can be a performance anti-pattern due to unnecessary memory allocation.

## 2025-05-13 - Perceived Performance and Color Schemes
**Learning:** Using the `<meta name="color-scheme" content="light dark">` tag allows the browser to immediately render the initial canvas in the user's preferred theme, even before CSS is parsed. This eliminates the "Flash of Unstyled Content" (FOUC) for dark-mode users, significantly improving perceived performance.
**Action:** Always include the color-scheme meta tag in the HTML head when supporting multiple themes to ensure a seamless initial render.

## 2025-05-14 - Content Containment for Landmarks
**Learning:** Upgrading landmark elements from `contain: layout` to `contain: content` provides combined layout and paint containment. This enables the browser to skip painting off-screen content entirely, further reducing GPU and main-thread overhead during scroll and resize events.
**Action:** Favor `contain: content` for top-level semantic landmarks that are expected to be visually self-contained, as it offers more aggressive rendering optimizations than layout containment alone.

## 2025-05-14 - Skip Layout and Paint with content-visibility
**Learning:** While `contain: content` optimizes the painting process, `content-visibility: auto` allows the browser to skip BOTH layout and paint for an element (and its children) when it's off-screen. This is even more powerful for long pages, as it reduces the initial work needed before the first frame can be rendered. Pairing it with `contain-intrinsic-size` prevents layout shifts when the element enters the viewport.
**Action:** Use `content-visibility: auto` for off-screen components, especially footers or secondary content sections, to minimize the browser's rendering work on initial load and during scroll.
