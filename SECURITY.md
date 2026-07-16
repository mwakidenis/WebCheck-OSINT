# Security Policy

## Supported Versions

We provide security updates for the latest stable release. Older versions may not receive patches.

| Version | Supported          |
| ------- | ------------------ |
| 1.x     | :white_check_mark: |
| < 1.0   | :x:                |

## Reporting a Vulnerability

WebCheck-OSINT is an OSINT tool that interacts with external websites and APIs. If you discover a security vulnerability – whether in the codebase, dependencies, or in how the tool handles user data – please **do not** create a public issue.

Instead, send a detailed report to **security@webcheck-osint.dev** (replace with your actual contact). Include:

- A clear description of the vulnerability.
- Steps to reproduce (with proof-of-concept if possible).
- Potential impact (e.g., data exposure, remote code execution, SSRF).
- Any suggested mitigation.

We will acknowledge your report within 48 hours and work on a fix.

## Responsible Disclosure

We follow standard responsible disclosure:

- Allow us 90 days to address the issue before public disclosure.
- Do not exploit the vulnerability beyond what is necessary for testing.
- Use only test environments; do not target production instances.

## Security Considerations for Users

- WebCheck-OSINT makes requests to third‑party websites. Ensure you have permission to scan the targets you investigate.
- The tool does not store any data by default, but if you enable logging or caching, be aware that sensitive information (e.g., headers, responses) may be recorded.
- Always run the tool in a secure environment and avoid exposing its API or UI to untrusted networks.

## Security Best Practices for Developers

- Keep dependencies up-to-date (`npm audit` regularly).
- Sanitize all user inputs to prevent injection attacks (e.g., command injection, XSS).
- Use environment variables for secrets – never hard-code.
- Implement rate limiting and request timeouts to avoid abuse.
- Run the application with the least privileges necessary.

We appreciate your efforts to keep WebCheck-OSINT secure for the community.
