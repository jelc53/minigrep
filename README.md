Simple version of classic command line utility `grep` from Rust handbook

**Idea**: `grep` searches a specified file for a specified string and prints any lines with that string.

**Main features include**:
- Takes command line arguments of a file path and a string
- Read environment variables to allow user to configure behaviour
- Print error messages to the standard error console stream (`stderr`) instead of standard output (`stdout`) so that user can redirect successful output to a file while still seeing error messages onscreen
