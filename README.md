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
rustlings                # watch mode: checks on every file save
rustlings run intro1     # run a single exercise (next pending if no name given)
rustlings check-all      # check everything, marking exercises done or pending
rustlings hint intro1    # show a hint
rustlings reset intro1   # reset an exercise to its original state
```

## Notes

- The workspace `Cargo.toml` wires up both `exercises/` and `solutions/` as binaries (`<name>` and `<name>_sol`).
- Clippy is configured as the check command via `rust-analyzer.toml`, matching how the Rustlings checker grades.
