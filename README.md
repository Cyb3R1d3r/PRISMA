# PRISMA

**PRISMA** (Platform Repair, Inventory, Status, Maintenance & Availability) is a fleet readiness platform for managing incidents/repairs, operational knowledge (lessons learned), logistics traceability, and availability across platforms (ships/aircraft/vehicles) with hierarchical role-based access.

## Repository structure
- `backend/` — Spring Boot (Gradle) REST API
- `frontend/` — React app (planned)

## Status
Early development — currently bootstrapping repository, database, and backend foundations.

## Local Database Setup

PRISMA uses PostgreSQL for local development.

### Prerequisites
- PostgreSQL installed locally (v13+ recommended)

### Create database and user
Run the following commands in `psql` or pgAdmin:

```sql
CREATE USER prisma WITH PASSWORD 'CHANGE_ME';
CREATE DATABASE prisma OWNER prisma;
GRANT ALL PRIVILEGES ON DATABASE prisma TO prisma;
