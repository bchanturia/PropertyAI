# PropertyAI Product Blueprint

## Core principle
PropertyAI should behave like an AI property manager, not merely a CRM with an AI chat box.

### System of record
Organisation → Users → Portfolio → Properties → Units → Tenancies → Tenants.

Operational records connect to Documents, Compliance, Inspections, Repairs, Contractors, Payments and Communications.

### Agent layer
AI receives goals/events and can use controlled tools: read property/tenancy/compliance/rent data; create tasks; request tenant availability; contact approved contractors; schedule inspections; draft communications; generate documents; log outcomes; escalate.

### Approval policy
Level 1 — autonomous: routine reminders, acknowledgements, task creation, contractor chasing, appointment coordination and record updates.

Level 2 — approval: quotes, non-routine expenditure, compensation, rent changes, sensitive complaint responses and contractor changes.

Level 3 — human mandatory: legal/possession actions, litigation, major commitments, serious safety incidents and decisions requiring legal interpretation.

Every action should produce an audit event containing actor, trigger, tool/action, timestamp, input context, result and approval state.

## MVP modules
1. Dashboard
2. Properties
3. Tenants and tenancies
4. Compliance
5. Repairs
6. Contractors
7. Rent and arrears
8. Inspections
9. Documents
10. Communications
11. AI Command Centre
12. Approval queue
13. Audit log

## Non-functional requirements
- Multi-tenant organisation isolation
- Role-based access
- MFA-ready authentication
- Immutable-style audit history
- Encryption in transit and at rest
- Backups and recovery
- Idempotent workflow execution
- Configurable jurisdiction rules
- Provider-agnostic AI orchestration
