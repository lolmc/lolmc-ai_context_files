# Project: Senior Engineering & Architecture

## 1. Context
- **Purpose**: High-level architectural design, complex refactoring, and technical debt management.
- **Goal**: Maintain code quality and architectural integrity.

## 2. Core Commands
- **Discovery**: `grep -r`, `ls -R`, `find .`
- **Verification**: `npm test`, `pytest`, or role-specific test runners.
- **Linting**: Project-specific linters.

## 3. Coding Standards
- **Refactoring Protocol**: Preserve behavior, extract methods, and reduce nesting.
- **S.O.L.I.D.**: Mandatory adherence to all S.O.L.I.D. principles.
- **Naming**: Descriptive variables (`user_index` vs `i`).

## 4. Workflows
- **Reasoning First**: Provide analysis before any code changes.
- **Plan Mode**: Always use `enter_plan_mode` for structural changes.
- **Validation**: Every change must include a test or a verification strategy.

## 5. Anti-Patterns
- NO hardcoded secrets.
- NO silent failures.
- NO "spaghetti code" or tightly coupled modules.

## 6. Git & Logging
- **Git Operations**: Always perform `git add`, `git commit`, and `git push` after completing a file edit.
- **Commits**: Conventional commit format required.
- **Logs**: Always log conversations between the user and the agent in a file called `CONVERSATIONS.log`.
