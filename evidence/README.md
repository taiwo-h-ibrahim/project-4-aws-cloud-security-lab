# Evidence Directory

This directory contains selected screenshots and reports supporting the AWS Cloud Security Lab exercises.

## IAM Least-Privilege Testing

- IAM policy configuration
- Successful S3 listing and object-read operations
- Denied S3 upload and deletion operations
- CloudTrail IAM management-event records

See [iam-least-privilege-policy.md](iam-least-privilege-policy.md) for the test procedure and results.

Supplementary policy and CLI evidence notes are retained in [hti-s3-least-privilege-evidence.md](hti-s3-least-privilege-evidence.md). The report above is the primary investigation record.

## IAM Account Access Review

- Review of the AWS-managed `AccountFullAccessRole` permissions and trust relationship
- Selected CloudTrail `ConsoleLogin` observations
- MFA/session-context interpretation and limitations
- Follow-up recommendations and evidence gaps

See [iam-account-access-review.md](iam-account-access-review.md). The review is inconclusive and does not claim that compromise was confirmed or definitively ruled out.

## S3 Security Controls

The following AWS console screenshots document the S3 security configuration:

- [Permissions and Security Settings](s3-permissions-security-settings-redacted.png)
  - Block Public Access enabled.
  - Bucket owner enforced.
  - ACLs disabled.

- [Properties, Encryption and Versioning](s3-properties-encryption-versioning-redacted.png)
  - Bucket versioning enabled.
  - Default SSE-S3 encryption.
  - Bucket Key enabled.

These screenshots are point-in-time configuration evidence.

S3 object-level CloudTrail data events were not enabled during this lab. CloudTrail observations are therefore limited to the management events documented in the relevant investigation report.

Sensitive credentials, secret keys, session tokens, MFA secrets, account identifiers, and unnecessary personal information must not be published. Sanitize screenshots and event exports before adding them to the public repository.
