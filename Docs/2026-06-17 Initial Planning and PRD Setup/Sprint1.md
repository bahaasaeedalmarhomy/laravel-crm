# Sprint 1: Foundation & Core Entities

**Goal**: Set up the infrastructure and provide basic CRUD for Contacts and Companies.

## Tasks

### 1. Infrastructure (Day 1-2)
- [ ] Initialize Laravel 11 project.
- [ ] Set up Docker (Laravel Sail) or local environment.
- [ ] Install `archtechx/tenancy` and configure multi-database tenancy.
- [ ] Set up a "Central" domain and a mechanism to create new tenants.

### 2. UI & Auth (Day 3)
- [ ] Install Filament PHP.
- [ ] Configure Filament to work within the tenant context.
- [ ] Set up basic branding (colors, logo).

### 3. Data Layer (Day 4)
- [ ] Database migrations for `Companies` (name, industry, website).
- [ ] Database migrations for `Contacts` (first_name, last_name, email, phone, company_id).
- [ ] Define Eloquent relationships and factories.

### 4. Core Features (Day 5-7)
- [ ] Create Filament Resources for `Company` and `Contact`.
- [ ] Implement "Global Search" across contacts and companies.
- [ ] Basic "Timeline" or "Activity Log" (Spatie Activitylog) for contacts.

## Success Criteria
- A developer can create a new tenant via command line or central panel.
- A user can log in to a tenant-specific URL (e.g., `tenant1.app.test`).
- A user can create, read, update, and delete Companies and Contacts within their tenant.
