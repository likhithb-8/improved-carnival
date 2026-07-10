# Bolt Performance Journal

## 2026-06-29 - Hardware-Accelerated Animations
**Learning:** Animating `box-shadow` triggers the Paint stage of the rendering pipeline on every frame, which can be expensive. Replacing it with `transform` and `opacity` on pseudo-elements allows the animation to be handled by the Compositor, often leading to 60fps even on lower-end devices.
**Action:** Prefer `transform` and `opacity` for continuous animations. Use `isolation: isolate` to manage stacking contexts when using negative z-index or absolute positioning for these effects.
