---
name: check
description: Validates your project structurally and with compiler-backed checks. Catches circular dependencies, orphaned files, layer violations, and type/syntax errors.
---

# Check the Codebase

This command validates the entire codebase and performs structural and compiler-backed checks. It catches circular dependencies, orphaned files, layer violations, and type/syntax errors.

`cxgrd check `

Compiler verification is currently supported for TypeScript, Python, and Rust
Compiler-backed verification works only if the compiler for the language is installed on the system.

## Available Options 
`--staged` — Only check git staged files.

`--changed` — Only check staged and unstaged changed files.

`--skip-compiler` — Skip compiler-backed verification.

`--skip-structural` — Skip structural graph checks.

`--strict` — Strict mode. Fail if a detected language compiler was skipped instead of just warning.