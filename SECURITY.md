# Security Policy

This policy applies to public repositories in the GoForj organization unless a
repository publishes a more specific policy.

## Supported versions

GoForj provides security fixes for the latest published release of each
maintained repository and for the default branch. A repository without a
published release is supported at its default branch only.

Older releases do not receive routine backports. When a confirmed vulnerability
affects an older release, the advisory will identify the affected versions, the
first fixed version, and any available mitigation. Consumers should plan to stay
on the latest release and treat an upgrade as the normal remediation path.

Generated application source is owned by the adopting application after it is
created. GoForj will assess whether a framework or template vulnerability
affects generated projects and will publish migration guidance when action is
required, but application teams remain responsible for applying and deploying
that change.

## Reporting a vulnerability

If the [GoForj private vulnerability reporting form](https://github.com/goforj/.github/security/advisories/new) is available, please use it. Private vulnerability reporting must be enabled in GitHub before the form can accept a report. Otherwise, email [chris@milestech.co](mailto:chris@milestech.co). Do not open a public issue, discussion, or pull request containing vulnerability details.

Include the affected repository and version or commit, a clear description of the impact, steps to reproduce, and any suggested mitigation. Reports that include a proof of concept should use only systems and data you are authorized to test.

If GitHub does not let you submit the form, use the email address above. Do not disclose vulnerability details publicly.

## What to expect

We aim to acknowledge a report within three business days and provide a status update at least every seven days while it is being investigated. We will confirm the affected scope, work on a fix or mitigation, coordinate a disclosure timeline with you when appropriate, and publish credit only with your permission.

We prioritize confirmed findings by practical impact, exploitability, affected
scope, and available mitigations. Severity scores inform triage but do not
replace this analysis.

| Severity | Remediation target |
| --- | --- |
| Critical | Provide containment or mitigation within 7 calendar days and target a fixed release within 14 calendar days. |
| High | Target a fixed release within 30 calendar days. |
| Moderate | Target a fixed release within 90 calendar days. |
| Low | Address in a planned maintenance release or document why no change is required. |

These are response targets, not guarantees. Upstream availability,
compatibility constraints, or coordinated disclosure may require a different
timeline. When that happens, maintainers will record the rationale, owner,
mitigation, and next review date in the private advisory or tracking record.

## Resolution and disclosure

A confirmed finding remains open until affected repositories and module paths
have been assessed, a fix or documented mitigation is available, relevant tests
and security checks pass, and the affected and fixed versions are known.

Public advisories identify impact, affected versions, fixed versions, and
migration or mitigation steps. Vulnerability details remain private until a fix
is available or coordinated disclosure requires publication. Maintainers may
release sooner when active exploitation or user safety makes early disclosure
necessary.

## Security update expectations

Security fixes may require dependency, configuration, or runtime changes. The
release or advisory will distinguish source compatibility, configuration
changes, persisted-data changes, minimum Go version changes, and operational
migration steps. Consumers are responsible for validating and deploying the
fix in their own environment.

Please give us reasonable time to investigate and remediate before sharing details publicly. We will not pursue legal action for good-faith research that avoids privacy violations, service disruption, destructive testing, and access to data or systems beyond what is necessary to demonstrate the issue.
