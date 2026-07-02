# Sentinel's Journal - Critical Security Learnings

## 2026-06-29 - Removed Ineffective CSP frame-ancestors from Meta Tag
**Vulnerability:** Security Misconfiguration (Ineffective Directive)
**Learning:** Browsers ignore the `frame-ancestors` directive when delivered via an HTML `<meta http-equiv="Content-Security-Policy">` tag. It must be sent via an HTTP response header to be effective.
**Prevention:** Always verify which CSP directives are supported in meta tags versus headers. Use HTTP headers for `frame-ancestors`, `report-uri`, and `sandbox`.
