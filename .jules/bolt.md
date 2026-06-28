## 2026-06-24 - Optimizing Off-screen Content Rendering
**Learning:** Applying `content-visibility: auto` to footer elements allows the browser to skip layout and paint for off-screen content, which is more efficient than `contain: layout` alone. Using `contain-intrinsic-size` prevents layout shifts when the element enters the viewport.
**Action:** Use `content-visibility: auto` for large, non-critical landmarks like footers to improve rendering performance.
