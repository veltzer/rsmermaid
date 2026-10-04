# TOFIX

Findings from a code scan on 2026-10-04.

## Medium

- `src/main.rs:2` - the crate is still a "Hello, World!" stub (the only test, line 12, just calls `main()`), yet it has been released up to v0.1.5 with `publish = true` (`release.toml:15`) and `README.md:2` says "A subset of mermaid implemented in Rust"; either implement a first mermaid subset before the next release or state in README/`docs/src/introduction.md` that the project is a placeholder and stop cutting releases.

## Low

- `README.md:2` - the README (and `docs/src/introduction.md:3`) have no usage, supported-syntax or install section, and disagree with each other ("A subset of mermaid implemented in Rust" vs "Rust version of mermaid"); document what the tool accepts and outputs once it does something.
