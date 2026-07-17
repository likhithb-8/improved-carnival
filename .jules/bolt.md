# Bolt's Journal

## 2026-07-02 - GPU Composite-only Status Badge Pulse
**Learning:** Animating CSS `box-shadow` forces the browser to run expensive Paint stages on every frame, which can cause frame drops and high CPU usage. Moving the animation to hardware-accelerated properties (`transform` and `opacity`) on pseudo-elements allows the browser to perform the animations entirely in the GPU's Composite stage, achieving 60fps and keeping CPU usage low.
**Action:** Use `transform` and `opacity` with `will-change: transform, opacity` to optimize pulse/glow animations instead of using `box-shadow` keyframes.
