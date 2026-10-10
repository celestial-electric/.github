# Celestial Electric repository governance

**Document:** CEL-GH-POL-001 · **Version:** 1.0 · **Steward:** Celestial Electric organization owners

## Purpose and scope

Maintain a clear, reviewable record of the software, documentation, automation, and monitoring work supporting Celestial Electric. Apply this baseline to new work while preserving repository-specific instructions and any stricter approved authority, review, data, or release requirements.

This policy describes expected practice. GitHub settings determine which controls are technically enforced. Neither a GitHub role nor this document grants authority to operate equipment, change production systems, spend money, contact customers, or accept a release outside the approved task scope.

## Repository stewardship

- Organization owners approve repository creation, deletion, transfer, and changes between public and private visibility. Record the purpose and affected repository before such changes.
- Keep business systems and internal operational records private. Public repositories contain only material approved for public release, with customer details and confidential implementation information removed.
- Before making a repository public, review the complete history, attachments, issues, and configuration for sensitive material and confirm publication rights. Removing a secret from the latest revision alone is insufficient.
- Prefer archiving a retired repository after reviewing retention needs. Deletion requires an owner decision and a verified recovery or retention plan.
- Give each repository a clear purpose, maintainer, README, support route, and appropriate local instructions. Use descriptive `celestial-` names for product repositories; GitHub special-purpose repositories such as `.github` are exceptions.

## Access and automation

- Use individual accounts, secure two-factor authentication, and the minimum access needed for assigned work. Do not share credentials or reviewer identities.
- Owners approve access and integrations. Record what each integration needs and which repositories it can access; review access when a person's role or an integration's purpose changes.
- Keep secrets in approved secret stores. Use synthetic or redacted examples in source control and review discussions. Never commit customer records, recovery codes, credentials, or confidential commercial information.
- Automation operates only within its approved scope. A passing workflow does not grant additional authority, and an owner exception does not count as independent review.

## Change and review

1. Identify the affected capability and its existing repository. Check local instructions and the current coordination record before starting overlapping work.
2. Make changes on a focused branch and submit a pull request with the problem, intended behavior, scope, evidence, and remaining limitations.
3. Preserve required checks and repository-specific approval requirements. Do not disable a failing gate or label unresolved evidence as a pass.
4. For production, access, security, data, or field-impacting changes, obtain review from a person independent of the author. A second account controlled by the same author is not independent review.
5. Tie review and verification to the actual version being accepted. Material changes after review require renewed review of the changed scope.

## Release and field readiness

- State the target environment, affected systems, migration or data impact, rollback approach, and accountable approver before a release.
- Distinguish built, connected, deployed, and verified states. Report an unknown or blocked result plainly and link the evidence that supports a claim.
- Follow each repository's approved release sequence. Merge, deployment, successful tests, and production acceptance are separate events.
- Monitoring software does not replace listed protective equipment or field commissioning. Changes affecting electrical equipment require qualified review and the applicable commissioning process before field use.
- Preserve receipts, readback evidence, review references, and closeout records in their approved locations. Public summaries should contain only information cleared for publication.

## Exceptions and policy changes

Record an exception's owner, reason, exact scope, duration, compensating controls, and closure evidence in the appropriate private project record. Escalate conflicts to the responsible owner rather than silently relaxing a requirement. Review this baseline when workflows, access, or responsibilities materially change.

Repository-specific licenses and rights remain attached to their respective projects. This policy does not change ownership, grant a license, or replace an executed agreement.
