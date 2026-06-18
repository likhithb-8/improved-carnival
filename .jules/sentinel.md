## 2024-06-20 - Standardized Vulnerability Disclosure with security.txt
**Vulnerability:** Lack of standardized, machine-readable vulnerability disclosure information.
**Learning:** While `SECURITY.md` is great for humans on GitHub, `security.txt` (RFC 9116) is the internet standard for vulnerability disclosure. It helps security researchers quickly find how to report issues, especially when the project is accessed outside of the GitHub UI.
**Prevention:** Always include a `.well-known/security.txt` file in web projects to facilitate responsible disclosure.
