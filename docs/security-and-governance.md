# Security and Governance

This demo is designed around least privilege and real-world operational constraints.

## Principles

- Least privilege delegated permissions
- No hardcoded secrets or tenant identifiers
- Clear separation of user intent and privileged operations
- Defensive handling of Graph errors and policy-driven constraints

## Permissions

Permission selection depends on the organization’s PIM configuration and policies.
Document the exact delegated permissions required in `graph/permissions.md`.

## Operational Notes

- Expect policy-driven failures (approval required, max duration, MFA requirements)
- Surface meaningful errors to users without leaking sensitive details
- Consider audit logging patterns for production implementations
