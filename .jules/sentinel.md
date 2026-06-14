## 2024-06-12 - Strict Content Security Policy (CSP) Implementation
**Vulnerability:** XSS and Clickjacking risks.
**Learning:** Even static applications benefit from a strict CSP as a defense-in-depth measure. Moving inline styles to an external CSS file is essential for removing `'unsafe-inline'` from the CSP.
**Prevention:** Always prioritize externalizing CSS and JS to enable the strictest possible CSP.
