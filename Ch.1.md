Ch.1

* function in rust is sart with `fn`
* Macro in rust is end with `!`
* `rustc` and `cargo` are both tools to build binary
    * We can build a project using `cargo build`.
    * We can build and run a project in one step using `cargo run`.
    * We can build a project without producing a binary to check for errors using `cargo check`.
    * `cargo check` is much faster than `cargo build`, the former can be used during coding to make sure it program can be compiled
    * Instead of saving the result of the build in the same directory as our code, Cargo stores it in the *target/debug* directory.

* use `cargo build --release` to compile it with optimizations (an executable in *target/release*)



Ch.2

* function return `Ok` / `Err` to apply error handling
* Like Java, use `.` to do serialized operation
* Can not avoid dead loop(loop controlled by user)