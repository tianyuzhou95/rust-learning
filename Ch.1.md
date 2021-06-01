# The Book Tips

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



Ch.3

* Use `mut` to make variables mutable
* `const` 和 immutable var 还是有区别的，一方面是 `let` 和 `const` 不一样，另一方面是 constant 的 type 必须显式声明，constant 可以在任意位置（scope）被声明，且声明语句也必须是 constant expression
* Shadow，和 C++ 不同，Rust 可以使用 `let` 重复定义重名变量，此时会将之前的同名变量覆盖掉，但是**否会覆盖掉空间我暂时未知**，理论上在编译时应该会优化
* Rust & Integer overflow ([link](https://doc.rust-lang.org/book/ch03-02-data-types.html#integer-overflow))
* function `fn`
    * `->  <type>` return value claim
    * last line with no semicolon is the return value, or use `return` key word to claim return



Ch.4

* memory management - [ownership](https://doc.rust-lang.org/book/ch04-01-what-is-ownership.html#what-is-ownership) checking during compile time
* Each value in Rust has a variable that’s called its *owner*.
* There can only be one owner at a time.
* When the owner goes out of scope, the value will be dropped.

