# Security Policy

Eurosky builds and operates public-interest social web infrastructure on the AT Protocol, including services that hold people's identities and data. We take the security of that infrastructure and of our users seriously, and we are grateful to anyone who helps us find and fix problems responsibly.

This policy applies to every repository in the [eurosky-social](https://github.com/eurosky-social) GitHub organisation, unless a repository has its own `SECURITY.md`, and to the services Eurosky operates.

## Reporting a vulnerability

**Please do not report security vulnerabilities in public GitHub issues, pull requests, discussions or social media posts.**

Report them privately using either of these routes:

- **GitHub private vulnerability reporting** (preferred for issues in our code): open the affected repository, go to the **Security** tab and choose **Report a vulnerability**.
- **Email:** [security@eurosky.tech](mailto:security@eurosky.tech).

If you are not sure whether something is a security issue, report it privately anyway. We would rather receive a report that turns out to be harmless than miss one that matters.

### What to include

To help us triage quickly, please include as much of the following as you can:

- The affected repository, service or URL, and the version or commit if known.
- A description of the issue and its potential impact.
- Step-by-step instructions to reproduce it, or a proof of concept.
- Whether the issue is already known publicly or being actively exploited.
- How you would like to be credited, if at all.

Please write in English if you can; reports in Dutch, French or German are also welcome.

## What to expect

We are a small team, so these are targets rather than guarantees, but we will do our best to meet them:

| Stage                           | Target                                                                  |
| ------------------------------- | ----------------------------------------------------------------------- |
| Acknowledge your report         | Within 3 working days                                                   |
| Initial assessment and severity | Within 10 working days                                                  |
| Fix for critical or high issues | As fast as possible, normally within 30 days                            |
| Fix for medium or low issues    | In a regular release, normally within 90 days                           |
| Public disclosure               | Coordinated with you once a fix is available, by default within 90 days |

We will keep you informed of progress, may ask you for more information, and will tell you when the issue is fixed. With your permission, we will credit you in the release notes or security advisory.

Where a fix is needed in code we have adopted from upstream (for example the AT Protocol reference implementations, or the Bluesky social app on which Mu is based), we will coordinate with the upstream maintainers and may share the details of your report with them for that purpose.

## Scope

### In scope

- Source code in repositories owned by the eurosky-social organisation.
- Services operated by Eurosky, including:
  - the Eurosky PDS and account services at `eurosky.social`
  - the Eurosky Portal at `portal.eurosky.tech`
  - the EU-HAUL migration service at `move.eurosky.tech`
  - the Mu social app at `mu.social` (and `staging.mu.social`), built from [eurosky-social-app](https://github.com/eurosky-social/eurosky-social-app), including its edge functions and, once released, its mobile apps
  - other Eurosky-operated infrastructure on `eurosky.social`, `eurosky.tech` and `eurosky.network`

Examples of issues we especially want to hear about: authentication or OAuth flaws, account takeover, access to another person's data, privilege escalation, injection, cross-site scripting, server-side request forgery, leaking of tokens or credentials, flaws in account migration or identity (DID / handle) handling, and, in Mu, issues such as session or token leakage in the browser, content injection through posts or embeds, and bypasses of moderation or privacy settings.

### Out of scope

- Vulnerabilities in third-party services we do not operate (for example Bluesky's own services); please report those to their operators. Issues in unmodified upstream software (the AT Protocol reference implementations, or Bluesky's social app) are best reported to the upstream project, though we are happy to be copied in.
- Denial-of-service or load testing, spam, and social engineering or phishing of Eurosky staff or users.
- Reports from automated scanners without a demonstrated, realistic impact.
- Missing security headers, best-practice suggestions or version disclosure without a concrete exploit.
- Issues that require a compromised device, a malicious browser extension or physical access.
- Problems with your own account, such as being locked out or a lost password: contact Eurosky support instead.

## Testing guidelines and safe harbour

We will not pursue or support legal action against anyone who acts in good faith under this policy. To stay within it, please:

- Only test against accounts and data you own or have explicit permission to use. Create test accounts rather than accessing other people's.
- Do not access, modify, download or keep more data than is strictly needed to demonstrate the issue, and delete anything you obtained once you have reported it.
- Do not degrade or disrupt our services or other people's use of them.
- Give us a reasonable chance to fix the issue before disclosing it publicly.
- Comply with applicable law.

If in doubt about whether something is allowed, ask us first at [security@eurosky.tech](mailto:security@eurosky.tech).

We do not currently run a paid bug bounty programme.

## Supported versions

Unless a repository says otherwise, only the latest release and the current default branch receive security fixes. Operators of their own deployments should keep up to date with the latest release.

## Security advisories

Fixed vulnerabilities are published as [GitHub security advisories](https://docs.github.com/en/code-security/security-advisories) on the affected repository and noted in its changelog.
