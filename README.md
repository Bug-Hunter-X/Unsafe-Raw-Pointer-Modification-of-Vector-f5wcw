# Unsafe Raw Pointer Modification of Vector in Rust

This repository demonstrates a common error in Rust: using raw pointers to modify vectors. Raw pointers bypass Rust's ownership system, leading to potential memory safety issues.  The example shows how modifying a vector through a raw pointer can lead to unexpected behavior and data corruption, highlighting the importance of safe memory management practices in Rust.

## Bug Description
The `bug.rs` file contains Rust code that attempts to modify a vector using a raw pointer obtained via `as_mut_ptr()`.  While seemingly functional, this approach is unsafe and prone to data corruption. The solution demonstrates proper methods for modifying a vector's elements. 

## How to reproduce the bug
1. Clone the repository.
2. Navigate to the project's root directory.
3. Compile and run the `bug.rs` file: `cargo run`
4. Observe the unexpected output.

## How to solve the bug
The `bugSolution.rs` file shows how to safely modify the vector's elements in Rust, avoiding unsafe raw pointer manipulation.