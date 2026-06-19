# Security Policy

## Reporting a Vulnerability

We take the security of Pullminder seriously. If you discover a security
vulnerability, please report it responsibly.

**Do NOT open a public GitHub issue for security vulnerabilities.**

Instead, please email us at **security@pullminder.com** with:

- A description of the vulnerability
- Steps to reproduce the issue
- The potential impact
- Any suggested fixes (optional)

For sensitive disclosures, see [Encrypted disclosure](#encrypted-disclosure)
below to arrange a secure channel.

## Response Timeline

- **Acknowledgment**: Within 48 hours of receiving your report
- **Initial Assessment**: Within 5 business days
- **Resolution**: We aim to resolve critical vulnerabilities within 30 days

## Safe Harbor

We support good-faith security research and will not pursue legal action
against researchers who:

1. Make a good-faith effort to avoid privacy violations, destruction of data,
   and interruption or degradation of our services.
2. Only interact with accounts they own or have explicit permission to access.
3. Do not exploit a vulnerability beyond what is necessary to demonstrate it,
   and do not exfiltrate, retain, or share data beyond a minimum proof of
   concept.
4. Give us a reasonable time to investigate and remediate before disclosing
   publicly (we ask for 90 days from the first contact, or earlier by mutual
   agreement).
5. Do not engage in social engineering of our staff, physical attacks against
   our offices, or attacks against our infrastructure providers.
6. Comply with all applicable laws.

If your activity follows these rules, we consider it authorised under the
Computer Fraud and Abuse Act and equivalent EU/Greek statutes, and will not
pursue or support a complaint with law enforcement. If a third party initiates
legal action against you for activity that complied with this policy, we will
make our authorisation known.

## Supported Versions

We provide security updates for the latest release of each package.

| Package | Supported |
|---|---|
| CLI (latest) | Yes |
| GitHub Action (v1) | Yes |
| Web application (`pullminder.com`, `app.pullminder.com`) | Yes |
| Marketing site (`pullminder.com`) | Yes |
| Documentation (`docs.pullminder.com`) | Yes |
| API (`api.pullminder.com`) | Yes |

## Scope

The following are in scope for security reports:

- The Pullminder CLI (`@pullminder/cli` on npm and the `pullminder` Homebrew
  formula).
- The Pullminder GitHub Action (available on the GitHub Marketplace).
- The Pullminder web application served from `pullminder.com` and
  `app.pullminder.com`.
- The marketing site, including any pages under `pullminder.com` and
  `*.pullminder.com`.
- The documentation site at `docs.pullminder.com`.
- The Pullminder API at `api.pullminder.com`.
- Public source repositories under the `pullminder` GitHub organisation.

The following are out of scope:

- Reports based solely on missing best-practice headers when no concrete
  exploit is demonstrated (please still report them, but do not expect a CVE).
- Denial-of-service attacks, including volumetric or protocol-level floods.
- Automated scanner output without manual verification.
- Vulnerabilities in third-party dependencies that are already publicly known
  and pending an upstream patch (we already monitor these).

## Encrypted disclosure

If your report contains sensitive information that should not traverse email
in plaintext, encrypt it to the PGP key below before sending to
`security@pullminder.com`.

### Key details

- **Fingerprint:** `EDA6 273A 22AE A269 7DAC 5A9D 8396 B06A ED47 3A30`
- **Type:** Ed25519 (sign/certify) + Curve25519 (encrypt) subkey
- **Created:** 2026-06-09
- **Expires:** 2027-06-09 (12-month rotation)

### Download

- [pullminder.com/.well-known/pgp/security.asc](https://pullminder.com/.well-known/pgp/security.asc)
- [keys.openpgp.org](https://keys.openpgp.org/vks/v1/by-fingerprint/EDA6273A22AEA2697DAC5A9D8396B06AED473A30)

### Import

```bash
curl -fsSL https://pullminder.com/.well-known/pgp/security.asc | gpg --import
```

Verify the fingerprint matches the one listed above before encrypting.

## Recognition

We appreciate security researchers who help keep Pullminder safe. With your
permission, we will acknowledge your contribution in our release notes and on
a public hall-of-fame page (planned for 2026).
