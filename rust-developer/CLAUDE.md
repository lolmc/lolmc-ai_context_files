# Project: Rust Development

## 1. Context
- **Purpose**: Systems programming, CLI tools, web services, and performance-critical applications in Rust.
- **Tech Stack**: Rust, Cargo, tokio, serde, clap, thiserror/anyhow.

## 2. Core Commands
- **Check**: `cargo check`
- **Build**: `cargo build` / `cargo build --release`
- **Test**: `cargo test`
- **Lint**: `cargo clippy -- -D warnings`
- **Format**: `cargo fmt --check`

## 3. Coding Standards
- **Ownership:** Respect borrowing rules. Prefer references over cloning where possible.
- **Error Handling:** Return `Result<T, E>` instead of panicking. Use `?` operator.
- **Naming:** Follow Rust conventions (snake_case for functions/variables, CamelCase for types).
- **Imports:** Group std, external crates, and local modules. Use `cargo add` for dependencies.

## 4. Workflows
- **Discovery:** Read `Cargo.toml` for dependencies, `src/lib.rs` or `src/main.rs` for entry points.
- **Validation:** Every public function must have at least one test. Run `cargo clippy` before committing.
- **Progress:** Commit after each logical sub-task with conventional commit messages.

## 5. Anti-Patterns
- NO `unwrap()` or `expect()` in non-test code without justification.
- NO `unsafe` blocks without `// SAFETY:` comment explaining invariants.
- NO `clone()` when a reference or `Cow` would suffice.
- NO silent error swallowing with `let _ =`.

## 6. Logs & Git
- **Conversations:** Record all significant user interactions in `CONVERSATIONS.log`.
- **Commit Format:** Follow Conventional Commits (`feat:`, `fix:`, `refactor:`, `test:`, `docs:`).
