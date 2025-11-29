# Security Policy

## Supported Versions

We actively support the following versions of the Virtual Business Card project:

| Version | Supported          |
| ------- | ------------------ |
| 1.0.x   | :white_check_mark: |

## Reporting a Vulnerability

We take security seriously. If you discover a security vulnerability in our Virtual Business Card project, please report it responsibly.

### How to Report

1. **Do NOT** create a public GitHub issue for security vulnerabilities
2. **Contact us directly** through one of these methods:
   - Email: Contact through our website form at [the-iah-creations.pages.dev](https://the-iah-creations.pages.dev/)
   - Direct message via LinkedIn (link available on the business card)

### What to Include

When reporting a security vulnerability, please include:

- **Description** of the vulnerability
- **Steps to reproduce** the issue
- **Potential impact** of the vulnerability
- **Suggested fix** (if you have one)
- **Your contact information** for follow-up

### Response Timeline

- **Initial Response**: Within 48 hours of report
- **Status Update**: Within 7 days with preliminary assessment
- **Resolution**: Security fixes will be prioritized and released as soon as possible

## Security Considerations

### Client-Side Security

This project is a client-side web application with the following security considerations:

#### Data Handling
- **No sensitive data storage**: The application doesn't store or process sensitive user data
- **External links**: All contact links are clearly visible and lead to legitimate platforms
- **QR code**: Points to the official website only

#### Content Security
- **External resources**: Uses trusted CDNs (Google Fonts, Font Awesome, QR Server API)
- **No user input**: The application doesn't accept or process user input
- **Static content**: All content is static HTML/CSS/JavaScript

### Recommended Security Practices

When hosting this business card:

1. **HTTPS**: Always serve over HTTPS in production
2. **Content Security Policy**: Consider implementing CSP headers
3. **Regular updates**: Keep any hosting platform updated
4. **Domain verification**: Ensure the QR code points to your verified domain

### Third-Party Dependencies

Current external dependencies:
- **Google Fonts**: fonts.googleapis.com, fonts.gstatic.com
- **Font Awesome**: cdnjs.cloudflare.com
- **QR Server API**: api.qrserver.com

All external resources are loaded from reputable CDNs with integrity checks where possible.

## Security Best Practices for Users

### For Developers
- Validate all external URLs before deployment
- Review any modifications to external resource URLs
- Test the application in a secure environment before deployment
- Keep local development environment secure

### For End Users
- Verify the authenticity of the business card URL
- Check that contact links lead to legitimate platforms
- Report any suspicious behavior or unexpected redirects

## Vulnerability Disclosure Policy

### Our Commitment
- We will acknowledge receipt of vulnerability reports
- We will provide regular updates on the status of reported vulnerabilities
- We will credit researchers who responsibly disclose vulnerabilities (if desired)
- We will not pursue legal action against researchers who follow responsible disclosure

### Scope
This security policy applies to:
- The main Virtual Business Card application (index.html)
- Associated CSS and JavaScript code
- Documentation and configuration files

### Out of Scope
- Issues with third-party hosting platforms
- General web security best practices not specific to this application
- Social engineering attacks
- Physical security of devices displaying the card

## Security Updates

Security updates will be:
- Released as patch versions (e.g., 1.0.1)
- Documented in the CHANGELOG.md
- Announced through our official channels
- Applied to all supported versions when possible

## Contact

For security-related questions or concerns:
- Visit our website: [the-iah-creations.pages.dev](https://the-iah-creations.pages.dev/)
- Use the contact methods provided on the business card
- Follow responsible disclosure practices

Thank you for helping keep our project secure! 🔒