# Bolt's Performance Journal ⚡

## Philosophy
- Speed is a feature
- Every millisecond counts
- Measure first, optimize second
- Don't sacrifice readability for micro-optimizations

## 2026-06-29 - Optimizing status indicator animations
**Learning:** Animating `box-shadow` (as seen in the status-badge pulse) is a 'Paint' operation and potentially less efficient than using composited properties like `transform` and `opacity` on pseudo-elements. Using `box-shadow` triggers expensive paint cycles on every frame of the animation.
**Action:** Replace `box-shadow` animations with `transform` and `opacity` on a separate pseudo-element (leveraging Composite phases via GPU) for smoother rendering. Apply `isolation: isolate` to the parent to manage z-index correctly for pseudo-elements with negative z-indices.
