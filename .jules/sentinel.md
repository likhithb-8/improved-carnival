## 2026-06-29 - Ineffective CSP Directives in Meta Tags
**Vulnerability:** Certain CSP directives, such as `frame-ancestors`, `report-uri`, and `sandbox`, are ignored by browsers when implemented via HTML `<meta>` tags.
**Learning:** CSP via meta tags has limitations compared to CSP delivered via HTTP headers. Including ineffective directives like `frame-ancestors` in a meta tag provides a false sense of security against clickjacking.
**Prevention:** Always deliver `frame-ancestors`, `sandbox`, and `report-uri` via HTTP response headers. Use meta tags only for directives that are supported, such as `default-src`, `script-src`, etc., and ensure a strict Referrer Policy is also set to protect user privacy.
