# minigrep
Implementation of minigrep as [taught](https://doc.rust-lang.org/book/ch12-01-accepting-command-line-arguments.html) in the Rust book

## Setup
1. Run `cargo build --release` in this repo's root directory to build the binary for your platform.
2. Add the `minigrep` binary compiled for your platform to your `PATH`.

## Usage
Perform a case-sensitive search by default
```bash
minigrep <query> <filename>

$ minigrep the ./poem.txt
```

To perform a case-insensitive search, set the `CASE_INSENSITIVE` environment variable. The actual value of this variable is irrelevant.
```bash
$ export CASE_INSENSITIVE=1
$ minigrep the ./poem
```