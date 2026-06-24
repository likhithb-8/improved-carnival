## 2025-06-24 - Ineffective CSP meta tag directive
**Vulnerability:** Use of `frame-ancestors 'none'` within a `<meta http-equiv="Content-Security-Policy">` tag.
**Learning:** The `frame-ancestors` directive is not supported when CSP is defined via an HTML meta tag. It must be delivered as an HTTP response header to be effective against clickjacking.
**Prevention:** Always implement `frame-ancestors` and `X-Frame-Options` at the server level (HTTP headers). Avoid adding them to meta tags to prevent a false sense of security.
