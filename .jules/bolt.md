## 2026-06-29 - Hardware-accelerated animations
**Learning:** Animations using 'box-shadow' trigger Paint and Layout cycles on every frame, which can be expensive for the main thread.
**Action:** Prefer 'transform' and 'opacity' for animations as they can be offloaded to the GPU's Composite stage.
