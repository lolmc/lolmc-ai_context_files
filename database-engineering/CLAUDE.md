# Project: Database Architecture & Engineering

## 1. Context
- **Purpose**: Schema design, data migration, and performance optimization.
- **Goal**: Maintain data integrity and scalable database performance.

## 2. Core Commands
- **Migration**: `migrate up`, `prisma migrate dev`.
- **Query Plan**: `EXPLAIN ANALYZE [query]`.
- **Backup**: `pg_dump -U [user] [db_name] > backup.sql`.
- **Lint/Check**: `sqlfluff lint [file]`.

## 3. Coding Standards (SQL & Migrations)
- **SQL**: Adhere to ANSI SQL; use clear, descriptive table and column names.
- **Migrations**: Always include a 'down' or 'rollback' script.
- **Performance**: Mandate appropriate indexing and avoid full table scans.

## 4. Workflows
- **Discovery**: Read current schema definitions (`schema.sql`, `prisma.schema`) before modification.
- **Safety**: Verify data consistency after every migration.
- **Verification**: Use query analysis to confirm performance improvements.

## 5. Anti-Patterns
- NO unversioned schema changes.
- NO database changes without a rollback path.
- NO storing sensitive data in plain text.

## 6. Logs & Git
- **Git Operations:** Always perform `git add`, `git commit`, and `git push` after completing a file edit.
- **Conversations:** Always log conversations between the user and the agent in a file called `CONVERSATIONS.log`.
- **Commit Format**: Follow Conventional Commits.
