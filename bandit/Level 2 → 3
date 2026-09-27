## Level 2 → 3

**Goal:** Find the password for the next level, stored in a file named `--spaces in this filename--`

**Approach:** Running `cat` on the filename unquoted caused the shell to split it on whitespace into several separate arguments, each treated as a missing file (`cat: --spaces: No such file...`, etc.). Adding `./` alone wasn't enough, since quoting hadn't been applied.

**Solution:** `cat "./--spaces in this filename--"` — quoting keeps the whole name as one argument, and `./` handles the leading dashes

**Takeaway:** Filenames with spaces must be quoted to be passed as a single argument; this compounds with the leading-dash problem from the previous level
