# Project: Python & Web Full-Stack

## 1. Context
- **Purpose**: Modern web application development using React, Next.js, and Python backends.
- **Tech Stack**: React, Next.js, TypeScript, Python, Pytest, Ruff.

## 2. Core Commands
- **Install**: `npm install` or `poetry install`.
- **Build**: `npm run build`.
- **Test**: `npm test`, `pytest`.
- **Lint/Fix**: `npm run lint --fix`, `ruff check . --fix`.

## 3. Coding Standards
- **React**: Functional components and arrow functions exclusively. Strict TypeScript.
- **Next.js**: Server Components by default; App Router patterns.
- **Python**: PEP 8 compliance, explicit typing, `Ruff` for all formatting.

## 4. Workflows
- **Discovery**: Read `package.json` or `pyproject.toml` to verify dependencies.
- **Validation**: Every new feature requires a unit test.
- **Progress**: Conventional commits and frequent pushes.

## 5. Anti-Patterns
- NO `any` types in TypeScript.
- NO silent exceptions in Python.
- NO default exports for React components.

## 6. Logs & Git
- **Conversations**: Mandatory record of all user interactions in `CONVERSATIONS.log`.
- **Commit Format**: Follow Conventional Commits.
