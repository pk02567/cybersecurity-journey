## Level 1 → 2

**Goal:** Find the password for the next level, stored in a file literally named `-`

**Approach:** `cat -` and `find -` both fail or hang, because `-` is interpreted as a flag/stdin marker rather than a filename — quoting it (`cat '-'`) doesn't fix this either, since the interpretation happens at the argument level, not the shell parsing level

**Solution:** `cat ./-` — prefixing with `./` forces the argument to be treated as a relative path, not an option

**Takeaway:** Command-line arguments starting with `-` need a path prefix to be read as filenames instead of flags
