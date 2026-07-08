## 2026-06-29 - Hardware-Accelerated Status Badge Animation
**Learning:** Animating `box-shadow` is a Paint operation that can cause layout/repaint cycles, impacting performance especially on low-powered devices. Using `transform` and `opacity` on a separate pseudo-element leverages the browser's compositor thread (GPU), ensuring a smooth 60fps animation without triggering expensive layout shifts or repaints.
**Action:** Always prefer composited properties (`transform`, `opacity`, `filter`) for continuous animations. Use `will-change` to hint for layer promotion when performance is critical.
