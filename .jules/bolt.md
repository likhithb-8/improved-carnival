## 2026-06-29 - Footer Rendering Optimization
**Learning:** For elements that are typically off-screen on initial load, such as footers, `content-visibility: auto` provides a significant performance boost by allowing the browser to skip layout and painting until the element is near the viewport.
**Action:** Use `content-visibility: auto` along with `contain-intrinsic-size` to optimize the rendering of off-screen landmarks and reduce initial rendering time.
