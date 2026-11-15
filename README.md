# Rustlings

My run through [Rustlings](https://github.com/rust-lang/rustlings), the official Rust exercises course.

**Status:** 94/94 exercises completed ✅

## Structure

| Directory | Description |
| --- | --- |
| `exercises/` | The exercises, as solved during the course |
| `solutions/` | Reference solutions |

Each exercise lives in its own topic folder — variables, move semantics, ownership, traits, lifetimes, smart pointers, threads, macros, conversions, and so on (24 topics plus 3 quizzes).

## Running

Requires the `rustlings` CLI (`cargo install rustlings`).

```sh
rustlings watch   # check all exercises on every file save
rustlings verify  # verify everything and stop on the first failure
rustlings run intro1
```

You can also run any single exercise with cargo directly:

```sh
cargo run --bin variables1
```

## Notes

- The workspace `Cargo.toml` wires up both `exercises/` and `solutions/` as binaries (`<name>` and `<name>_sol`).
- Clippy is configured as the check command via `rust-analyzer.toml`, matching how `rustlings verify` grades.
