## 2026-07-02 - Hardware-Accelerated Animations
**Learning:** Animating `box-shadow` or `border` triggers the Paint stage of the rendering pipeline, which is computationally expensive and can lead to jank. Using `transform` and `opacity` allows the browser to handle animations in the Composite stage, leveraging the GPU for much smoother performance (60fps).
**Action:** Always prefer `transform` and `opacity` for continuous animations. Use `will-change` to hint the browser for layer promotion when necessary.
