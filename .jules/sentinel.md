## 2024-06-12 - Strict Content Security Policy (CSP) Implementation
**Vulnerability:** XSS and Clickjacking risks.
**Learning:** Even static applications benefit from a strict CSP as a defense-in-depth measure. Moving inline styles to an external CSS file is essential for removing `'unsafe-inline'` from the CSP.
**Prevention:** Always prioritize externalizing CSS and JS to enable the strictest possible CSP.

## 2024-06-14 - Defense-in-Depth for Static Assets and Privacy
**Vulnerability:** Potential DOM-based XSS and information leakage via referrers.
**Learning:** Even without active scripts, using `require-trusted-types-for 'script'` in CSP provides a proactive defense against future DOM-XSS. Setting a strict Referrer Policy is a low-effort, high-impact privacy enhancement.
**Prevention:** Default to `strict-origin-when-cross-origin` and use Trusted Types directives in CSP for all new web projects.
