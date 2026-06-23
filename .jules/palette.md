## 2025-06-23 - Custom Scrollbar Implementation
**Learning:** Browser-native scrollbars often clash with dark mode or specific brand color palettes, creating a jarring visual experience. Using `scrollbar-width` and `scrollbar-color` provides a standard way to theme scrollbars in modern browsers, while `::-webkit-scrollbar` offers deeper customization for WebKit/Blink browsers.
**Action:** Always define scrollbar colors using CSS variables that respond to theme changes to ensure a cohesive look and feel across all components and modes.
