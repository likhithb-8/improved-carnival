## 2026-06-24 - Composite-Only Transitions
**Learning:** Properties like 'top' trigger the Layout and Paint stages of the browser rendering pipeline, which are expensive. Using 'transform' (e.g., translateY) moves the work to the Composite stage, which is handled by the GPU, ensuring 60fps animations and lower main-thread load.
**Action:** Always prefer 'transform' and 'opacity' for animations and transitions to maximize rendering performance.
