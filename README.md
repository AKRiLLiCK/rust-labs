<div align="center">

<img src="icon.png" alt="Rust Labs Logo" width="200"/>

# Rust Labs

**A playground of focused Rust experiments. Small, clear, practical.**  
*Made with love with Rust ❤️*

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Rust](https://img.shields.io/badge/rust-stable-e57324.svg)](https://www.rust-lang.org/)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)

[**Explore Labs**](#-labs) • [**How to Run**](#-getting-started) • [**Contribute**](#-contributing)

</div>

---

## 📘 Philosophy: Why This Exists

Rust mastery comes from **mental models**, not just syntax.

**Rust Labs** is a collection of self-contained experiments, each exploring a single Rust concept in isolation. It is designed for developers—especially those migrating from languages like C++, Python, or JavaScript—who want to internalize *how* Rust works, rather than just blindly writing code that compiles.

The goal is simple: **Teach by doing.**
*   ❌ No "fill in the missing semicolon" drills.
*   ✅ Minimal, runnable programs that you can break, fix, and analyze.
*   ✅ Deep explanations of "why" things crash or compile.

---

## 🚀 Getting Started

This repository is organized as a **Cargo Workspace**. You can run experiments from the root or navigate into specific labs.

### Prerequisites
*   [Install Rust](https://www.rust-lang.org/tools/install) (latest stable).

### Workflow
1.  **Clone the repo:**
    ```
    git clone https://github.com/AKRiLLiCK/rust-labs.git
    cd rust-labs
    ```

2.  **Pick a lab and run it:**
    *   *Option A (From Root):*
        ```
        cargo run -p ownership-moves
        ```
    *   *Option B (Navigate):*
        ```
        cd labs/ownership-moves
        cargo run
        ```

3.  **The most important step:**
    Open the source code (`src/main.rs`). Read the comments. Uncomment the "broken" lines to see the compiler errors yourself. **Break it, then fix it.**

---

## 🧪 Labs

Each lab focuses on a specific "Aha!" moment in the Rust learning curve.

| Concept | Directory | Focus & "Aha" Moment |
| :--- | :--- | :--- |
| **Ownership & Moves** | [`labs/ownership-moves/`](labs/ownership-moves/) | **The Core:** Stack vs. Heap. Why values "move" instead of copy. Understanding Drop semantics. |
| **Borrowing & Refs** | [`labs/borrowing/`](labs/borrowing/) | **The Rules:** Immutable `&T` vs Mutable `&mut T`. Visualizing aliasing rules that prevent data races. |
| **Lifetimes (Intro)** | [`labs/lifetimes-basic/`](labs/lifetimes-basic/) | **The Contract:** How the compiler tracks references. Why generic lifetime parameters exist. |
| **Pattern Matching** | [`labs/patterns/`](labs/patterns/) | **Control Flow:** Destructuring structs/enums. Match guards. Irrefutable vs. Refutable patterns. |
| **Traits & Generics** | [`labs/traits-generics/`](labs/traits-generics/) | **Polymorphism:** Rust's answer to interfaces. Trait bounds, `impl Trait`, and monomorphization. |
| **Error Handling** | [`labs/errors/`](labs/errors/) | **Safety:** `Result` vs `Option`. The `?` operator. Designing custom error enums properly. |
| **Iterators** | [`labs/iterators/`](labs/iterators/) | **Functional:** Lazy evaluation, adapters (`map`, `filter`), and Zero-Cost Abstractions. |
| **Concurrency** | [`labs/concurrency/`](labs/concurrency/) | **Threads:** `std::thread`, channels (`mpsc`), and shared state (`Arc<Mutex<T>>`). |
| **Modules** | [`labs/modules/`](labs/modules/) | **Structure:** Visibility (`pub`), module trees, and file system hierarchy. |

### 🚧 Upcoming Labs (Roadmap)
*   `async-await` (Tokio basics, Futures)
*   `smart-pointers` (`Box`, `Rc`, `RefCell` deep dives)
*   `unsafe` (Raw pointers and FFI)

---

## 🤝 Contributing

This is an **Open Sandbox**. Contributions are welcome!

The goal is not just to add code, but to add **clarity**. If you want to add a lab:
1.  **Keep it Focused:** One concept per lab.
2.  **Explain the "Why":** Comments should explain *why* the code behaves this way, not just what it does.
3.  **Include "Break Me" Sections:** clearly mark lines that users should uncomment to trigger interesting compiler errors.

Please open an issue to discuss a new lab before submitting a PR.

---

## 📄 License

MIT — Use, fork, learn, experiment.
