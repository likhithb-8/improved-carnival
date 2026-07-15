## 2026-07-14 - content-visibility for Off-screen Components

**Learning:** `content-visibility: auto` is superior to `contain: layout` for off-screen components (like footers). It allows the browser to skip layout and painting entirely until the element enters the viewport.
**Action:** Always pair with `contain-intrinsic-size` to prevent layout shifts during scrolling.
