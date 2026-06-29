## 2026-06-29 - Security Header Optimization
**Vulnerability:** Ineffective CSP directive and missing Referrer Policy.
**Learning:** The `frame-ancestors` directive in a CSP `<meta>` tag is ignored by browsers; it must be delivered via an HTTP response header. Additionally, a missing Referrer Policy can lead to information leakage during cross-origin requests.
**Prevention:** Use `strict-origin-when-cross-origin` to protect user privacy and configure server-level headers for frame protection.
