# Contributing to Rust Labs 🦀🧪

Welcome to Rust Labs — a personal sandbox for exploring Rust through experiments, notes, and tinkering.  
Whether you want to add a tiny lab or build a deeper experiment, the guiding principle is: **keep it meaningful, clear, and helpful**.

---

## 🧠 What Counts as a Contribution

### ✅ Simple Labs  
- A small crate (≈ 100–250 lines) focused on a **single concept**  
- Minimal, clear code that you can easily run, break, and explore  
- Optional `notes.md` for explanation, mental models, or “aha-moments”

### ⚙️ In-Depth Experiments or Engineering Labs  
- More ambitious labs that explore nontrivial Rust or systems-level ideas  
- Should include clear documentation and rationale (e.g. `notes.md`, comments, or read-through text)  
- Complexity is fine — as long as it leads to insight, clarity, or educative value (not just cleverness)  

**In short:** small and simple *or* intentionally deep and documented.  

---

## 🧪 What to Avoid  

- Cleverness or abstraction that hides understanding  
- Over-engineering for the sake of “looking sophisticated” without educational purpose  
- Labs that do too many unrelated things at once — clarity of concept matters  

---

## 🔧 How to Add a New Lab or Experiment

1. Inside `labs/`, run:  
```bash
   cargo new <lab-name> --bin
```

Choose a clear, concept-focused name (e.g. `ownership-moves`, `async-lifetimes`, `unsafe-ptrs`, etc.).

2. Add the new crate to the workspace by listing it in the root `Cargo.toml` under `members`.

3. Write the code:

   * For simple labs: minimal `main.rs`, small number of lines, easy to run or break.
   * For deeper experiments: code plus documentation (in `notes.md` or comments) explaining the purpose, trade-offs, and what you learn.

4. (Recommended) Add a `notes.md` in the lab directory, covering:

   * What the lab explores
   * Why the concept matters
   * What happens when you tweak or break things
   * What you learned or found interesting
   * Ideas for further experiments

5. (If adding a new lab) Optional: add a line in the main `README.md` table referencing the new lab.

---

## 🧰 Improving or Updating Existing Labs

* Simplify or clarify code where helpful
* Add or improve `notes.md` documentation to increase understanding
* Add “break-me” examples to clarify Rust behavior where appropriate
* If a lab grows in scope, consider splitting into multiple labs each focusing on a single concept

---

## ✔️ Checklist Before Submitting

* Lab has a clear purpose
* Concept is well-defined
* Code is small (for simple labs) or documented (for complex ones)
* If applicable, `notes.md` explains what this lab teaches or reveals
* Workspace setup reflects the new addition (if any)

If you’re unsure whether a change fits — a short GitHub issue describing the idea first is totally fine.

---

## 📄 License

All contributions follow the same MIT license as this repository.

Happy experimenting 🦀