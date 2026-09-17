<!--
Example context.md for the tutor skill. Copy this file to context.md and replace
the contents with your own — or just delete it and let the skill interview you.
Keep the section headings; they're what the skill parses. This example uses
learning Rust to show the skill is subject-agnostic.
-->

# Learning context

## Learner profile

- Backend developer, comfortable in Python and Go; new to systems programming.
- Prefers dense, exercise-first learning; little patience for padded tutorials.

## Subject

Rust, from fundamentals through building and shipping a real CLI tool.

## Sources (in study order)

1. *The Rust Programming Language* ("the book") — chapters read in order.
2. Rustlings exercises — done alongside the matching book chapters.
3. Jon Gjengset's "Crust of Rust" videos on YouTube for the topics the book waves
   at (traits, lifetimes, smart pointers).

## Destination

Be able to write a small production-grade CLI tool in Rust and read
common open-source Rust code without drowning in the borrow checker.

## Connect mapping (studied concept → destination)

- Ownership and borrowing → why APIs take `&str` vs `String`
- Result/`?` → error handling style in the CLI tool
- Traits → how to keep the tool's storage backend swappable

## Environment (practice machine)

- macOS, zsh. Allowed commands: `cargo new`, `cargo build`, `cargo test`,
  `cargo clippy`, `rustc --explain E0382` (and other error codes).
- No IDE required; terminal and editor are fine.

## Phases & milestones

- **Phase 1 — The book, chapters 1–10.** Milestone: implement a grep clone
  (chapter 12) from scratch without copying, explaining every lifetime annotation
  in it.
- **Phase 2 — Smart pointers, concurrency, testing (chapters 13–20).** Milestone:
  a small multi-threaded web server (chapter 20) that passes my own test suite.
- **Phase 3 — The CLI tool.** Capstone: publish a crate that does something I
  actually use, with tests and CI.

## Known simplifications in the source (don't test the loose version)

- The book defers `unsafe` almost entirely until chapter 19 — don't test it before.
- Early chapters imply `String` and `&str` are interchangeable in function
  signatures; the real distinction lands in chapter 4.

## Source style notes (calibration)

- The book is prose-heavy with worked projects; Rustlings is pure drills.
  Quizzes should lean on retrieval from the book but assign practice from
  Rustlings-style small exercises.
