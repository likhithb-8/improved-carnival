## 2025-06-12 - Hardware-Accelerated Transitions
**Learning:** Properties that trigger the "Layout" and "Paint" stages of the browser rendering pipeline (like `top`, `left`, `margin`, `height`) are significantly more expensive to animate than "Composite-only" properties like `transform` and `opacity`. Offloading these to the GPU via `transform` ensures smoother 60fps transitions and reduces main-thread load.
**Action:** Always prefer `transform` and `opacity` for animations and transitions. Use `will-change` judiciously; for infrequently used elements like "Skip to Content" links, it can be a performance anti-pattern due to unnecessary memory allocation.

## 2025-06-15 - Rendering Isolation with Layout Containment
**Learning:** The `contain: layout` CSS property isolates an element's layout from the rest of the document. This means the browser can optimize rendering by limiting the scope of reflows and repaints. When a change occurs inside a contained element, the browser doesn't necessarily need to re-calculate the layout for the entire page.
**Action:** Apply `contain: layout` (or `contain: content`) to top-level semantic landmarks and independent UI components to reduce the computational cost of DOM updates and improve overall rendering performance.
