## Level 5 → 6

**Goal:** Find one file among many nested subdirectories in `inhere` — matching three criteria: regular file, exactly 1033 bytes, not executable

**Approach:** Initial attempts had stray spaces breaking flag syntax (`- type`, `-typef`), which the shell couldn't parse correctly

**Solution:** `find . -type f -size 1033c ! -executable` returned `./maybehere07/.file2`; `cat` on that path revealed the password

**Takeaway:** `find` flags must be written without spaces between the dash and the flag name (`-type`, not `- type`); `find` can filter by type, exact size, and permission attributes simultaneously
