## 2026-06-29 - Hardware-Accelerated Animations
**Learning:** Animating `box-shadow` triggers expensive Paint cycles on every frame because the shadow must be recalculated. Using `transform` and `opacity` allows the browser to offload animations to the GPU Composite stage, significantly reducing Main thread work and improving FPS.
**Action:** Replace `box-shadow` animations with pseudo-elements that use `transform: scale()` and `opacity` for pulse effects.
