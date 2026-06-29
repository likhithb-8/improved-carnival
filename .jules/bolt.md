## 2026-06-29 - Off-screen Rendering Optimization
**Learning:** Applying `content-visibility: auto` and `contain-intrinsic-size` (e.g., `auto 100px`) to the `<footer>` landmark provides superior performance to `contain: layout` alone by allowing the browser to skip both layout and paint calculations for off-screen content.
**Action:** Use `content-visibility: auto` for large, off-screen components like footers to improve initial page load and rendering performance.
