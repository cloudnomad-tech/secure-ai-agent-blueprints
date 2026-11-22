# Multi-Tenant AI Security

## Authentication

Use OAuth 2.0 and OpenID Connect for secure access.

Validate:

- Token issuer
- Token audience
- Expiration
- Required permissions

## Tenant Isolation

Every request must resolve an authorized tenant.

Recommended practices:

- Enforce tenant-scoped database queries.
- Validate resource ownership.
- Apply role-based access control.
- Prevent cross-tenant data access.

## AI Agent Security

Protect agent workflows by:

- Validating tool parameters.
- Restricting tool permissions.
- Applying least-privilege access.
- Logging sensitive tool operations.
- Requiring approval for high-risk actions.

## MCP Integration

MCP servers should implement:

- Scoped authorization
- Input validation
- Request auditing
- Tool allowlists
- Secure credential handling

## RAG Security

- Filter retrieved documents by user permissions.
- Enforce tenant isolation in vector searches.
- Prevent unauthorized document retrieval.
- Avoid storing sensitive data in logs.

## Operational Security

- Rotate application credentials.
- Use managed secret storage.
- Monitor suspicious activity.
- Establish audit retention policies.
