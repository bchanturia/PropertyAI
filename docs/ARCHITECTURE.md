# PropertyAI Architecture

## Target stack
- Next.js + TypeScript web application
- PostgreSQL relational database
- Object storage for certificates, photos, invoices and reports
- Background job/workflow engine
- Model-agnostic AI orchestration
- Email first; SMS/WhatsApp later

## Separation of concerns
**Rules engine:** deterministic deadlines, eligibility, required documents and escalation thresholds.

**AI layer:** classification, extraction, summarisation, drafting, prioritisation and tool selection.

**Workflow layer:** durable multi-step processes, retries, timeouts and scheduled actions.

**Approval layer:** explicit human decisions for controlled actions.

**Audit layer:** every mutation and AI decision traceable to an event.

## Initial database entities
- organisations
- users
- portfolios
- properties
- units
- tenants
- tenancies
- documents
- compliance_items
- inspections
- repairs
- contractors
- work_orders
- payments
- communications
- tasks
- approvals
- ai_runs
- audit_events

## Design rule
The AI never receives unrestricted database credentials. It acts through typed, permission-checked tools.
