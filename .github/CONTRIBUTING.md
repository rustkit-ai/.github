# Contributing to rustkit-ai

Thank you for your interest in contributing! We welcome contributions of all kinds — bug reports, feature ideas, documentation, and code.

## Getting started

1. **Fork** the repository and clone it locally
2. **Install Rust** via [rustup](https://rustup.rs) if you haven't already
3. **Build** the project: `cargo build`
4. **Run tests**: `cargo test`

## How to contribute

### Reporting bugs

Open an issue using the **Bug Report** template. Include:
- What you did
- What you expected
- What actually happened
- Your OS, Rust version (`rustc --version`), and tool version

### Suggesting features

Open an issue using the **Feature Request** template. Describe the problem you're solving, not just the solution.

### Submitting code

1. Open an issue first for non-trivial changes — alignment before implementation saves time
2. Create a branch from `main`
3. Keep commits focused and messages clear
4. Make sure `cargo test`, `cargo clippy`, and `cargo fmt --check` all pass
5. Open a pull request against `main`

## Code style

- Run `cargo fmt` before committing
- Run `cargo clippy -- -D warnings` and fix all warnings
- Prefer clarity over cleverness
- Keep public APIs minimal

## Commit messages

Use the conventional format:

```
feat: add semantic cache layer
fix: handle empty release list gracefully
docs: update install instructions
```

## License

By contributing, you agree that your contributions will be licensed under the same license as the project (MIT).