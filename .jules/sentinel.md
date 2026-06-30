## 2026-06-29 - CSP Meta Tag Directives Limitation
**Vulnerability:** Use of `frame-ancestors 'none'` within an HTML `<meta http-equiv="Content-Security-Policy">` tag.
**Learning:** Certain CSP directives, most notably `frame-ancestors`, `report-uri`, and `sandbox`, are ignored when delivered via a `<meta>` tag. They must be sent as an HTTP response header to be effective.
**Prevention:** Always implement `frame-ancestors` and other restricted directives at the server/infrastructure level via HTTP headers (e.g., `Content-Security-Policy: frame-ancestors 'none';`). Use `<meta>` tags only for a subset of directives when header control is unavailable, and document the limitations.
