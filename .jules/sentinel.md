## 2026-06-24 - Implement Referrer Policy
**Vulnerability:** Information leakage via the `Referer` header when navigating from the application to external sites.
**Learning:** Default browser behavior for referrers can expose sensitive internal URL structures or parameters to third-party domains.
**Prevention:** Explicitly set a `strict-origin-when-cross-origin` Referrer Policy to ensure only the origin is sent in cross-origin requests, while preserving full URL details for same-origin navigation.
