## Level 6 → 7

**Goal:** Find a file somewhere on the entire filesystem, owned by user `bandit7`, group `bandit6`, exactly 33 bytes

**Approach:** Home directory was empty, meaning the file wasn't local — needed to search the whole filesystem from `/` rather than `.`. Initial attempts also carried over the wrong size (1033c) from the previous level before correcting to 33c.

**Solution:** `find / -type f -user bandit7 -group bandit6 -size 33c 2>/dev/null` located `/var/lib/dpkg/info/bandit7.password`; `cat` on that path gave the password

**Takeaway:** When the home directory is empty, the target likely lives elsewhere on the system — search from `/`. Redirecting stderr (`2>/dev/null`) filters out permission-denied noise from an unrestricted filesystem search.
