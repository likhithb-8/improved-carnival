## 2026-07-14 - Optimized Rendering with content-visibility
**Learning:** `content-visibility: auto` is more powerful than `contain: layout` for off-screen components. While `contain: layout` limits the scope of browser work, `content-visibility: auto` allows the browser to skip layout and painting entirely for elements not currently in the viewport.
**Action:** Use `content-visibility: auto` for large or complex components that are likely to be off-screen (like footers or sections below the fold), and always pair it with `contain-intrinsic-size` to prevent layout shifts.
