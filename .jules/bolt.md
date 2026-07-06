## 2026-06-29 - Inefficient Pulse Animation using Box-Shadow
**Learning:** Animating `box-shadow` is a 'Paint' operation that can be expensive because it triggers a repaint of the element and potentially its surroundings on every frame.
**Action:** Use composited properties like `transform` and `opacity` on pseudo-elements to create similar effects. This moves the animation to the 'Composite' stage, which is handled by the GPU and doesn't trigger Layout or Paint, resulting in smoother animations and less main-thread work.
