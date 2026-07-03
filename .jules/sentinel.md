## 2026-06-29 - Ineffective CSP Directives in Meta Tags
**Vulnerability:** Inclusion of 'frame-ancestors' directive in a CSP <meta> tag, providing a false sense of clickjacking protection.
**Learning:** Browsers ignore framing, sandboxing, and reporting directives when delivered via <meta> tags; these must be implemented as server-sent HTTP headers.
**Prevention:** Use meta-CSP only for content source directives (e.g., script-src); remove ineffective directives from HTML to maintain configuration clarity.
