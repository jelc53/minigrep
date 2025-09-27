# introduction

**Idea**: `grep` searches a specified file for a specified string and prints any lines with that string.

**Main features include**:
- Takes command line arguments of a file path and a string
- Read environment variables to allow user to configure behaviour
- Print error messages to the standard error console stream (`stderr`) instead of standard output (`stdout`) so that user can redirect successful output to a file while still seeing error messages onscreen


# getting started

To run the program from source, use the following commands:
```
  cd minigrep
  cargo run -- <query> <file_path>
```

- *query* is the text string you are searching for
- *file_path* is the path (from root directory) to the file you wish to search
