# The rust programming language


## 01,02,03 lectures Introduction, Installing, Hello, Rust!

### What's rust?

1. It's new programming language
2. Made by the Mozilla corporation
3. Already had a 1.0 release
4. Produces native code
5. Powerful and safe
6. Modern and fast
7. An alternative C/C++, D, Go, ....
8. Introduces new and interesting concepts

- Types and Variable
- Control Flow
- Data Structures
- Functions
- Lifetime
- Docs and Tests

### Installing and Configuration

https://www.rust-lang.org/

*Using asdf:*

```sh
1. add the plugin
asdf plugin-add rust https://github.com/code-lever/asdf-rust.git

2. list all rust available options
asdf list all rust

3. choose the version
asdf install rust 1.75.0

4. Use it globally
asdf global rust 1.75.0

5. Check it is installed
rustc --version
rustc --help
```

### Hello Rust!

1. Please create a file named hello.rs. Add the following code:
```
fn main()
{
    println!("Hello, Rust!")
}
```
2. Compile the file with `rustc hello.rs`, a executable file named `hello` will be created.
3. Run the executable file with `./hello`.
4. The output should be `Hello, Rust!`





