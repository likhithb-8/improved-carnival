# Bolt's Performance Journal

## 2026-06-29 - Optimization of Off-screen Content
**Learning:** `contain: layout` limits the scope of reflows, but `content-visibility: auto` provides a more significant performance boost by allowing the browser to skip layout and paint entirely for off-screen elements.
**Action:** Use `content-visibility: auto` for large or complex footer/header elements that are likely to be off-screen on initial load, paired with `contain-intrinsic-size` to prevent layout shift.
