# Rust Data Race Example

This repository demonstrates a common error in Rust: creating multiple mutable borrows of the same variable.  This leads to a runtime panic because Rust's borrow checker cannot guarantee memory safety in this scenario.

The `bug.rs` file contains the erroneous code. The `bugSolution.rs` file offers a possible fix.  Understanding the root cause of this issue is crucial for writing safe and concurrent Rust code.