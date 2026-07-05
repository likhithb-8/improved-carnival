## 2026-06-29 - Hardware-Accelerated Animations
**Learning:** Animating properties like `box-shadow` or `width`/`height` triggers 'Paint' and 'Layout' operations, which are computationally expensive and run on the main thread. Using `transform` (for scale/translation) and `opacity` allows the browser to handle animations during the 'Composite' stage, leveraging the GPU for smoother 60fps performance and reduced CPU overhead.
**Action:** Always prefer `transform` and `opacity` for continuous animations. For pulse effects, use a pseudo-element with `transform: scale()` instead of `box-shadow`.
