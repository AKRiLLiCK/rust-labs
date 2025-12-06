# Rust Labs
![alt text](https://github.com/AKRiLLiCK/rust-labs/blob/b56d4031d63a7336e51f24454a8597e30e9380bc/icon.png)

*A sandbox of small, focused Rust experiments designed to build intuition through practice.*

Rust Labs is a collection of self-contained “labs,” each exploring one core Rust concept in isolation — ownership, traits, lifetimes, iterators, error handling, concurrency, and more.  
The idea is simple: create minimal programs that do one thing clearly and use them to form an internal model of how Rust really works.

Made with love with Rust ❤️

---

## Index of Labs

Each directory contains:
- a description of the concept  
- a minimal Rust example  
- notes on what the experiment revealed  

As you progress you’ll add entries like these:

### **Ownership & Moves**
`labs/ownership-moves/`  
How values move, copy, and drop. Why some types copy implicitly and others don’t.  
Hands-on playground for understanding Rust’s value semantics.

### **Borrowing & References**
`labs/borrowing/`  
Exploring shared references `&T`, mutable references `&mut T`, aliasing rules, and compiler restrictions.

### **Lifetimes (Intro)**
`labs/lifetimes-basic/`  
What lifetimes actually represent and why they exist. Minimal examples without diving into advanced patterns.

### **Pattern Matching**
`labs/patterns/`  
Destructuring, guards, binding, irrefutable vs. refutable patterns, and how match arms are checked.

### **Traits & Generics**
`labs/traits-generics/`  
Custom traits, trait bounds, generic functions, blanket impls, and type inference quirks.

### **Error Handling**
`labs/errors/`  
Using `Result`, `?`, custom error enums, mapping functions, and thinking about how Rust expresses failure.

### **Iterators**
`labs/iterators/`  
Creating custom iterators, chaining adapters, lazy evaluation, and how iterator combinators shape data flow.

### **Concurrency**
`labs/concurrency/`  
Threads, channels, shared-state synchronization, and early async experiments.

### **Modules & Project Structure**
`labs/modules/`  
Understanding visibility, module trees, file layout, and how crates fit together.

---

## How to Use This Repo

1. Pick a concept you want to understand.  
2. Enter its corresponding lab directory.  
3. Run it, modify it, break it, rebuild it.  
4. Add notes reflecting what you discovered.  

Labs should be small enough to finish in under two hours but deep enough to produce “aha” moments.

---

## Why This Exists

Rust mastery comes from forming strong *mental models*, not memorizing syntax.  
These labs help develop those models through experimentation and iteration — perfect for personal learning, future guides, or teaching others.

---

## License

MIT, so anyone can learn from and contribute to these experiments.
