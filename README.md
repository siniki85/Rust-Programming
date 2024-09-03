# Rust-Programming

## Getting Started
Let’s start your Rust journey! There’s a lot to learn, but every journey starts somewhere. In this chapter, we’ll discuss:

### Installing Rust on Windows
Writing a program that prints Hello, world!
Using cargo, Rust’s package manager and build system

The first step is to install Rust. We’ll download Rust through rustup, a command line tool for managing Rust versions and associated tools.

### Installing rustup on Windows
On Windows, go to https://www.rust-lang.org/tools/install and follow the instructions for installing Rust. 

**To check whether you have Rust installed correctly, open a shell and enter this line:**

$ rustc --version

**You should see the version number, commit hash, and commit date for the latest stable version that has been released, in the following format:**

rustc x.y.z (abcabcabc yyyy-mm-dd)

**If you see this information, you have installed Rust successfully! If you don’t see this information, check that Rust is in your %PATH% system variable as follows.
In Windows CMD, use:**

> echo %PATH%

## Hello, Cargo!
Cargo is Rust’s build system and package manager. Most Rustaceans use this tool to manage their Rust projects because Cargo handles a lot of tasks for you, such as building your code, downloading the libraries your code depends on, and building those libraries. (We call the libraries that your code needs dependencies.)

**If you installed Rust through some other means, check whether Cargo is installed by entering the following in your terminal:**

$ cargo --version

**Creating a Project with Cargo:**

$ cargo new Project_Name
$ cd Project_Name

**Building and Running a Cargo Project:**

$ cargo build
$ .\target\debug\hello_cargo.exe 


**We just built a project with cargo build and ran it with ./target/debug/hello_cargo, but we can also use cargo run to compile the code and then run the resultant executable all in one command:**

$ cargo run

**Cargo also provides a command called cargo check. This command quickly checks your code to make sure it compiles but doesn’t produce an executable:**

$ cargo check
