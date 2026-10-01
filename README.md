# PropertyAI

AI-first property management operating system.

## Product direction
PropertyAI is designed as an AI letting/property-management operator: the portfolio database is the system of record, deterministic workflows enforce rules, AI handles routine reasoning and communications, and humans approve consequential actions.

## Prototype
The first interactive prototype is in `index.html` and is intentionally dependency-free so it can be deployed as a static site.

## Roadmap
- Portfolio/property/tenant/tenancy data model
- Compliance engine with versioned jurisdiction rules
- Repairs and contractor workflows
- Rent and arrears automation
- AI command centre and approval queue
- Communications and document generation
- Audit trail and permissions
- Production backend, authentication, PostgreSQL and workflow orchestration

## Safety
Legal/compliance decisions must be driven by versioned jurisdiction rules and approval controls rather than unconstrained model output.
