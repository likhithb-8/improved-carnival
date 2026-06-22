## 2026-06-22 - CSP Meta Tag Limitations
**Vulnerability:** Ineffective clickjacking protection via meta tag CSP.
**Learning:** The `frame-ancestors` directive is ignored by browsers when delivered via a `<meta http-equiv="Content-Security-Policy">` tag. It must be delivered as an HTTP response header.
**Prevention:** Always use HTTP headers for frame protection (`X-Frame-Options` or `Content-Security-Policy: frame-ancestors ...`) and do not rely on meta tags for these specific directives.
