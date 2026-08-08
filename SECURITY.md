# Security Policy

## 🛡️ Supported Versions

We actively maintain and provide security updates for the following versions of **Draw On Screen With Laser**:

| Version | Supported          | Notes |
| ------- | ------------------ | ----- |
| Latest Release (v1.x) | :white_check_mark: | Recommended version |
| Older Pre-releases   | :x:                | Please update to the latest release |

---

## 🔒 Security & Privacy Overview

**Draw On Screen With Laser** is designed with user privacy and system security as top priorities:
- **100% Offline Operation:** The application does not collect, record, or transmit personal data, screen recordings, or input content to external servers.
- **Overlay Permissions:** The app uses Android's `SYSTEM_ALERT_WINDOW` permission solely to render the floating canvas overlay and floating widget toolbar.
- **Screen Privacy:** The canvas floating layer passes touch events through when in minimized/view mode and does not intercept sensitive credential entries outside the active drawing canvas.

---

## ⚠️ Reporting a Vulnerability

We take the security of our application and users seriously. If you believe you have discovered a security vulnerability or privacy defect, please follow these steps:

### How to Report

1. **Do NOT open a public GitHub issue** for security vulnerabilities.
2. Send an email describing the vulnerability to the repository owner or submit a private security advisory via [GitHub Security Advisories](https://github.com/rishibanota/draw-on-screen-with-laser/security/advisories/new).
3. Include detailed information to help us reproduce the issue:
   - Type of vulnerability (e.g., permission escalation, overlay hijacking vulnerability, memory leak).
   - Step-by-step instructions to reproduce the issue.
   - Proof-of-concept code or demonstration video (if applicable).
   - Affected Android versions and device hardware.

---

## ⏱️ Response Timeline

When a security report is submitted:

- **Initial Response:** Within **48 hours**, acknowledging receipt of your report.
- **Triage & Evaluation:** Within **5 business days**, confirming the vulnerability and establishing its severity rating.
- **Patch Release:** Security patches will be prioritized and published in a release update as soon as possible.
- **Public Disclosure:** Once a fix is verified and released, we will credit the security researcher (unless anonymity is requested) in the release notes.

---

## 🚫 Out of Scope

The following issues are considered out of scope for security reports:
- Issues requiring physical root access to an unlocked target device.
- Issues related to third-party Android ROM modifications not present in stock Android.
- Theoretical attacks without practical proof-of-concept.

Thank you for helping keep **Draw On Screen With Laser** safe and secure for everyone!
