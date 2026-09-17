<!--
Example trusted-resources.md for the tutor skill. Copy this file to
trusted-resources.md and replace the contents with your own — or just delete it
and let the skill interview you on first use. Keep the three sections
(Knowledge / Wisdom / Gaps) and the per-entry fields; they're what the skill
parses. This example continues the Rust scenario from context.example.md.

Sources (what you're studying and being quizzed on) live in context.md. This
file is for authorities the tutor should ground its *answers* in when you ask a
question — links, books, transcripts, docs — plus the communities it can route
judgment calls to, and the topics no resource covers yet.
-->

# Trusted resources — Rust

## Knowledge

## The Rust Programming Language ("the book")

- Type: book / website
- Locator: https://doc.rust-lang.org/book/ (print: No Starch Press, 2nd ed.)
- Scope: language semantics — ownership, borrowing, traits, error handling,
  concurrency. The authority when my notes and the book disagree.
- Access: fetch the URL for the relevant chapter.

## Crust of Rust transcripts

- Type: transcript
- Locator: trusted-resources/crust-of-rust/ (one .txt per talk, tactiq-style)
- Scope: deep dives the book waves at — lifetimes, traits, smart pointers.
- Access: read the matching transcript file.

## Rust standard library docs

- Type: docs
- Locator: https://doc.rust-lang.org/std/
- Scope: exact API signatures and behavior of standard library items. Look here
  before answering any "what does this method actually return" question.
- Access: fetch the URL for the specific item.

## Wisdom (communities)

## users.rust-lang.org

- Locator: https://users.rust-lang.org/
- Use for: "is this the idiomatic way to do X?" judgment calls. Attempt an
  answer first; route here to confirm or when the tutor's knowledge runs out.

## Gaps

- Async runtime internals — how a scheduler like tokio's actually works. The
  book defers async; no deep resource picked yet. Candidate: Jon Gjengset's
  async-focused Crust of Rust episodes.
- Embedding Rust on microcontrollers — interesting, but off-mission for the
  CLI-tool goal; deliberately not looking for a resource.
