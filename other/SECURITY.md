# Security Policy

## About This Policy

SciCat is a community-driven, volunteer-maintained open source project. There is no commercial entity operating SciCat, no dedicated security team, and no service-level agreement (SLA) attached to this policy. Response times described below are best-effort targets, not guarantees.

This document describes how the SciCat maintainers and steering committee handle the discovery, triage, and disclosure of security issues in the upstream project — it does not cover the operational security of any individual deployment.

## Reporting a Vulnerability

If you believe you've found a security vulnerability in SciCat, please **do not open a public GitHub issue**. Instead, report it privately using one of the following channels:

- Raise a private PR or Issue that will notify the SciCat adminsitrators
- Create a private Slack channel with the SciCat Project leads

Please include as much of the following as you can:

- A description of the vulnerability and its potential impact
- Steps to reproduce, or a proof-of-concept
- Affected version(s), component(s), or deployment configuration
- Any known mitigations

We will acknowledge receipt of your report as soon as a maintainer is available to do so — typically within a few business days, given the project's volunteer nature.

## Severity Classification

We classify reported issues into three severity levels. Classification is judgment-based and considers exploitability, impact (data exposure, integrity, availability), and whether exploitation requires privileged access.

### Low Severity
Issues with minimal practical impact — for example, issues requiring unusual local access, exposing non-sensitive information, or requiring significant, unlikely preconditions to exploit.

### Medium Severity
Issues that could lead to limited unauthorized access, data exposure, or disruption under realistic conditions, but that are constrained in scope (e.g., affecting a single component, requiring authentication, or needing specific configurations to be exploitable).

### High Severity
Issues that could lead to significant unauthorized access, data loss/exposure, remote code execution, authentication/authorization bypass, or broad service disruption, and that are exploitable under common or default configurations.

Severity is assessed by the maintainers/steering committee and may be revised as more information becomes available.

## Our Response Process

Regardless of severity, all confirmed vulnerabilities follow the same disclosure sequence:

1. **Private notification to the Steering Committee.** Once a report is triaged and confirmed, the SciCat steering committee members are notified privately so that adopting sites represented on the committee have early visibility and can begin preparing to respond internally.
2. **Fix development.** Maintainers develop and test a patch, coordinating privately with reporters and steering committee contacts as needed.
3. **Public release.** Once a fix is ready, it is released through the normal SciCat release channels, accompanied by a public advisory describing the issue (with technical detail added only after the fix has had a reasonable chance to be adopted).

Adopting sites are strongly encouraged to subscribe to release notifications and to have their own patching process in place as part of their SLOs, since the project itself does not push updates to deployments.

### Target Response Times (Best Effort)

| Severity | Initial Acknowledgment | Steering Committee Notification | Target Fix & Public Release |
|----------|------------------------|----------------------------------|------------------------------|
| High     | 1–3 business days      | As soon as confirmed             | As soon as practical; expedited effort from available maintainers |
| Medium   | Up to 5 business days  | Within the same window as confirmation | Next reasonable release cycle, or sooner if maintainer capacity allows |
| Low      | Up to 5 business days  | Included in routine steering committee updates | Bundled into a regular release |

These timeframes reflect a volunteer effort and depend on maintainer availability. There is no contractual or business-criticality obligation behind them.

## Disclosure

We follow a coordinated disclosure approach: details are not published until a fix is available, except where a vulnerability is already public or actively being exploited, in which case we will notify the steering committee and adopting community as quickly as possible, even ahead of a fix, so sites can apply their own mitigations.

We credit reporters in the public advisory unless they request otherwise.

## Supported Versions

[Insert table of currently supported/patched versions, e.g.:]

| Version | Supported |
|---------|-----------|
| latest  | ✅ |
| LTS | ✅ |

## Scope

This policy covers the SciCat core codebase and components maintained under the SciCat GitHub organization. It does not cover:

- Vulnerabilities in third-party dependencies (please report these upstream, though letting us know is appreciated so we can track and update)
- The security configuration or operation of any specific institutional deployment of SciCat

## Questions

For anything not covered here, reach out via the SciCat Slack Channel.
