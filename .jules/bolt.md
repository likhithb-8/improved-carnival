## 2026-06-29 - Animating Box-Shadow vs Composited Properties
**Learning:** Animating `box-shadow` (as seen in the status-badge pulse) triggers 'Paint' operations on every frame. This is a CPU-intensive operation that can lead to dropped frames. By switching to a pseudo-element that animates `transform` and `opacity`, the work is moved to the 'Composite' stage (GPU), which is much more efficient.
**Action:** Always prefer composited properties like `transform` and `opacity` for continuous animations to maintain 60fps and reduce main-thread load.
