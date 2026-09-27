## Level 4 → 5

**Goal:** Find the password among 10 files in `inhere`, only one of which is human-readable text — the rest are junk/binary data

**Approach:** `ls -l` showed all 10 files with identical size and permissions, so listing alone didn't distinguish them. Used `file ./-file*` to check each file's actual type.

**Solution:** `file` identified `-file07` as `ASCII text` (the rest were `data`); `cat ./-file07` printed the password

**Takeaway:** `file` inspects actual content/type rather than relying on name, size, or permissions — useful when files are deliberately made to look identical
