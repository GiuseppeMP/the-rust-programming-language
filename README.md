# The rust programming language


## 01,02,03 lectures - Introduction, Installing, Hello, Rust!

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

**Using asdf:**

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

## 04 lecture - Introducing the Cargo Package Manager

To build and manage Rust projects, Cargo is a tool that helps you manage your dependencies and build your project.

Rust have some conventions:

1. Have a Cargo.toml file in the root of the project
2. Have a Cargo.lock file in the root of the project
3. Have a src folder in the root of the project
4. Should exists a file named main.rs in the src folder

**Introducing with Cargo manually:**

1. Create a directory named `my-project`
2. Create a file named `my-project/Cargo.toml`
3. Create a file name `src/main.rs`
4. Write the following code in `src/main.rs`:
```rust
fn main()
{
    println!("Hello, World!")
}
```
5. Write the following code in `Cargo.toml`:
```toml
[package]
name = "hello-world"
version = "0.1.0"
authors = [ 'Beppe<email@example.com>' ]
```
6. Instead of running `rustc src/main.rs`, now we should use `cargo build`
7. A folder filed `target`, should be created in the root of the project
8. Run the executable file with `cargo run`.
9. The output should be `Hello, World!`


**Using Cargo commands**

You can generate the same project using cargo commands.

1. To create a executable and not a library use: `cargo new hello-world --bin` 
2. It should create a folder named `hello-world` containing subfolders `src`, `Cargo.toml`, and `Cargo.lock`.
3. If you remove `--bin` from the command, it generates a library instead of an executable.
