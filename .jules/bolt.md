## 2026-07-02 - Hardware-Accelerated Pulse Animation
**Learning:** Animating properties like 'box-shadow' or 'border' triggers expensive Paint stages. Hardware acceleration via 'transform' and 'opacity' offloads animation work to the GPU's Composite stage, achieving 60fps and reducing CPU load.
**Action:** Always favor 'transform' and 'opacity' paired with 'will-change' for continuous visual animations to prevent layout shifts and paint thrashing.
