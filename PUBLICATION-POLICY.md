# GSLHub Public Documentation Policy

Public documentation should explain enough to support scientific review, collaboration and software reuse without exposing unnecessary operational risk.

## Publish when

A document is suitable for `gslhub/docs` when it:

- explains architecture, interfaces, workflows or governance at a public-safe level;
- supports reproducibility or contributor understanding;
- contains no credentials or secrets;
- avoids unnecessary personal/server identifiers;
- does not expose restricted research records or raw evidence;
- has a clear canonical owner and version/context;
- can be maintained without duplicating a canonical document elsewhere.

## Keep private or sanitize when

A document contains:

- credentials, API tokens or connection strings;
- private host paths or account identifiers that add no public value;
- backup/restore details that materially increase operational exposure;
- private participant or researcher data;
- unreleased research artifacts or evidence;
- third-party confidential information;
- incident details whose publication could create ongoing security risk.

Sanitization should preserve the methodological or architectural value while replacing environment-specific values with placeholders such as `<host-user>`, `<domain>`, `<secret>` or `<storage-path>`.

## Canonical-source rule

Do not duplicate long documents just to make them visible in another repository. Link to the canonical source whenever possible.

## Historical documentation

Outdated but scientifically relevant documentation may be retained when clearly marked with the version/date it describes. Operationally obsolete runbooks should not be presented as current guidance.

## Security issues

Potential security vulnerabilities should follow the organization security policy rather than being disclosed through ordinary public documentation changes.
