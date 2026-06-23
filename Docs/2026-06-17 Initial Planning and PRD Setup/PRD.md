# Product Requirement Document (PRD) - Agent-Native CRM

## 1. Executive Summary
An "Agent-Native" CRM built on Laravel, designed specifically to be easily controlled by AI Agents (via MCP or structured APIs) while providing a top-tier human experience through Filament/Livewire.

## 2. Target Audience
Initially a generic CRM for small-to-medium businesses, with architecture ready to be "skinned" for specific niches.

## 3. Scope (MVP)

### In-Scope
- **Multi-Tenancy**: Data isolation for different companies using a multi-database approach.
- **Core CRM Entities**:
    - **Contacts**: Individual people.
    - **Companies**: Organizations contacts belong to.
    - **Leads**: Potential sales opportunities.
    - **Deals**: Qualified leads in a pipeline.
- **Sales Pipeline**: A Kanban board for managing deals through stages.
- **Role-Based Access Control (RBAC)**: Admin, Manager, Rep.
- **Agent-Native Foundation**: Structured JSON APIs for all core entities.

### Out-of-Scope (Version 1)
- Advanced Marketing Automation.
- Complex AI Scoring (manual scoring first).
- Customer Support Ticketing.
- Third-party Integrations (Stripe, Xero, etc.).

## 4. Technical Stack
- **Backend**: Laravel 11
- **Frontend**: Filament PHP (Livewire 3)
- **Database**: PostgreSQL (Recommended for robust multi-tenancy)
- **Real-time**: Laravel Reverb
- **Tenancy**: `archtechx/tenancy`

## 5. User Roles
- **System Admin**: Manages tenants/companies.
- **Tenant Admin**: Manages users within their company.
- **Sales Rep**: Manages their own contacts, leads, and deals.
