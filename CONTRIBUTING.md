# Contributing to Rust Labs 🦀🧪

Rust Labs is a small playground of experiments, notes, and Rust ideas.
Everything here exists because someone wanted to explore how Rust works — by *doing*, *breaking*, or *tweaking* code.

If you want to add something, follow the same spirit:
**keep it tiny, focused, curious, and fun.**

---

## 🧠 What’s a “Lab”

A lab is:

* a small crate (usually under ~150–200 lines)
* exploring **one** Rust concept
* intentionally minimal — no frameworks, no heavy structure
* written so you can poke at the code and instantly see what breaks or changes
* accompanied by a short note explaining the “aha” moment the code illustrates

Labs are *not*:

* full applications or end-user programs
* “clean architecture” patterns or complex abstractions
* code that values cleverness over clarity
* style wars, over-engineering, or rigid structure

This repo is about intuition, not polish.

---

## 🔧 How to Add a Lab

### 1. Create a new crate

From inside `labs/`:

```
cargo new <lab-name> --bin
```

Pick a simple, meaning-focused name (e.g. `ownership-moves`, `lifetimes-basic`, `iterators-map`).

### 2. Add it to workspace

Include it in the root `Cargo.toml` under the workspace’s members.

### 3. Write the lab

Each lab should have:

* a small `main.rs` (or minimal module structure)
* comments that explain what's going on
* ideally, at least one “break this” example to demonstrate compiler behavior or runtime error
* code focusing on a single concept — nothing extra

Suggested minimal layout:

```rust
//! Lab: <name>
//! Goal: What this lab is about.
//! Concept: The Rust idea under investigation.

fn main() {
    println!("Rust Lab: <name>");

    // Working example

    // --- BREAK THIS to see what happens ---  
    // let x = ...; // causes compile-time error or undefined behavior
}
```

### 4. Update the README

Add one line in the labs table:

```
| <Concept> | `labs/<lab-name>/` | <One-line explanation> |
```

---

## 🧪 Improving or Refactoring Existing Labs

Small adjustments are welcome — e.g.:

* clearer comments
* simpler or more illustrative examples
* better “break-me” cases
* cleanup of unnecessary code

If you want to broaden the scope too much — split into separate labs so each stays focused.

---

## ✔️ Quick Checklist Before Submitting

* Lab is small (approx. ≤ 200 lines)
* Focuses on a single concept
* Contains at least one illustrative “break-me” or minimal error-triggering example
* Code runs (or fails intentionally) — that failure illustrates something real
* README table updated (if adding a new lab)

If you’re unsure: better to open an issue first and sketch the idea.

---

## 📄 License

By contributing, you agree that your work is under the same MIT license as this repository.

Happy experimenting 🦀🎉