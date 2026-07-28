# Security Policy

## Reporting a Vulnerability

If you discover a security vulnerability — either in [herline.vip](https://herline.vip) or in any public repository under the `herline` GitHub organization — please report it **privately**:

📧 **<security@herline.vip>**

**Please do not open a public GitHub issue for security vulnerabilities.**

## What to Include

When reporting, please share as much as you can:

- **Type of issue** (e.g., XSS, SSRF, auth bypass, data exposure, dependency vulnerability)
- **Location** — URL path, API endpoint, or file path
- **Steps to reproduce** — numbered, clear, concise
- **Impact assessment** — what an attacker could do
- **Environment** — browser, OS, any relevant details
- **(Optional) Suggested fix** — if you have ideas
- **(Optional) Proof-of-concept** — screenshots, sanitized logs, minimal repro code

## Our Commitment

We take every report seriously. Here's what you can expect:

| Stage | Timeline |
| --- | --- |
| Initial acknowledgment | Within **48 hours** |
| Triage & severity assessment | Within **7 days** |
| Status update | Every **7 days** until resolved |
| Public disclosure (if applicable) | Coordinated with reporter |

**We will:**

- Keep you informed as we investigate and fix
- Credit you in our security advisories (unless you prefer to stay anonymous)
- **Not pursue legal action** against researchers acting in good faith
- Coordinate responsible disclosure timing with you

## Scope

### In scope

- **[herline.vip](https://herline.vip)** and all subdomains
- **Public repositories** under the `herline` GitHub organization
- **Herline mobile apps** (when released)
- **Herline API endpoints** (public and authenticated)

### Out of scope

- Third-party services we integrate with (report to them directly)
- Social engineering attacks on Herline staff
- Physical security of our offices
- Denial of service via volumetric attacks
- Issues in unsupported or end-of-life software
- Self-XSS requiring user to paste hostile code into their own browser console
- Clickjacking on pages without sensitive actions
- Missing best-practice headers where no vulnerability is demonstrated

## Safe Harbor

We consider security research conducted under this policy to be:

- Authorized in accordance with the Computer Fraud and Abuse Act (CFAA)
- Authorized in accordance with the EU's NIS2 Directive (to the extent applicable)
- Exempt from DMCA 1201 restrictions on circumventing technical controls

Research that follows this policy and our coordinated disclosure timeline will be considered authorized. We waive any Herline-initiated DMCA claim against you for circumventing Herline's technical measures.

## Bug Bounty

We don't currently run a formal bounty program, but we deeply appreciate responsible disclosure and will publicly credit contributors (with their permission) in our security advisories and acknowledgments page.

If you report a critical vulnerability, we'll do our best to express our gratitude meaningfully — reach out and let's talk.

---

Thank you for helping keep Herline and its users safe.
