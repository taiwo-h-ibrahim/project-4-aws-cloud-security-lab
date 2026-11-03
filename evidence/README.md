# Evidence Directory

This directory contains selected screenshots and reports supporting the AWS Cloud Security Lab exercises.

## IAM Least-Privilege Testing

- IAM policy configuration
- Successful S3 listing and object-read operations
- Denied S3 upload and deletion operations
- CloudTrail IAM management-event records

See [iam-least-privilege-policy.md](iam-least-privilege-policy.md) for the test procedure and results.

## IAM Account Access Review

- Review of the AWS-managed `AccountFullAccessRole` permissions and trust relationship
- Selected CloudTrail `ConsoleLogin` observations
- MFA/session-context interpretation and limitations
- Follow-up recommendations and evidence gaps

See [iam-account-access-review.md](iam-account-access-review.md). The review is inconclusive and does not claim that compromise was confirmed or definitively ruled out.

## S3 Security Controls

The lab documentation records the following S3 configuration observations:

- S3 Block Public Access
- Default server-side encryption using SSE-S3
- Bucket versioning
- Object Ownership set to Bucket owner enforced, with ACLs disabled

**Publication status:** Supporting screenshots for these S3 configuration settings are not currently present in this repository. The two published S3 screenshots support the IAM policy configuration and denied upload test only. Do not treat the configuration observations above as independently verified by the current screenshot set. Add sanitized console screenshots if they are available; otherwise retain the qualification in the project README.

Sensitive credentials, secret keys, session tokens, MFA secrets, account identifiers, and unnecessary personal information must not be published. Sanitize screenshots and event exports before adding them to the public repository.
