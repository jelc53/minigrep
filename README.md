# introduction

**Idea**: `grep` searches a specified file for a specified string and prints any lines with that string.

**Main features include**:
- Takes command line arguments of a file path and a string
- Read environment variables to allow user to configure behaviour
- Project structured into modules and crates (binary and library) to match rust best practices
- Print error messages to the standard error console stream (`stderr`) instead of standard output (`stdout`) so that user can redirect successful output to a file while still seeing error messages onscreen


# getting started

To run the program from source, use the following commands:
```
  cd minigrep
  cargo run -- <query> <file_path>
```

- *query* is the text string you are searching for
- *file_path* is the path (from root directory) to the file you wish to search

For example, `cargo run frog poem.txt` should return one line to the terminal *"How public, like a frog"*.

To ignore case, you can pass the environment variable `IGNORE_CASE=1` either with a `.env` file or directly in the terminal.


# debugging

Standard output (`stdout`) is either written to file `> output.txt` or to console if output path omitted. Error messages (`stderr`) are always written to console.

Before making any changes, run `cargo test` from the project root directory to ensure current tests are passing.

