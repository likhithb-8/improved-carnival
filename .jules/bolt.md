## 2026-07-02 - Animating box-shadow triggers expensive Repaint/Paint stages
**Learning:** Animating properties like `box-shadow` or `border` triggers expensive Paint stages in the rendering pipeline on every frame, which can cause CPU spikes, especially on low-end devices. Hardware acceleration via `transform` and `opacity` offloads animation work to the GPU's Composite stage, achieving 60fps and reducing CPU load.
**Action:** Replace `box-shadow` pulse animations with separate pseudo-elements (`::before` and `::after`) animated independently via GPU-composited `transform` and `opacity` properties. Always use `will-change: transform, opacity` to hint the browser for layer promotion.

## 2026-07-14 - content-visibility: auto for Off-Screen Components
**Learning:** `content-visibility: auto` is superior to `contain: layout` for off-screen components (like footers). It allows the browser to skip layout and painting entirely until the element enters the viewport.
**Action:** Pair `content-visibility: auto` with `contain-intrinsic-size` to prevent layout shifts during scrolling on non-critical off-screen components.
