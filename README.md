# minigrep
Implementation of minigrep as [taught](https://doc.rust-lang.org/book/ch12-01-accepting-command-line-arguments.html) in the Rust book

## Setup
Add the `minigrep` binary compiled for your platform to your `PATH` environment variable.

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