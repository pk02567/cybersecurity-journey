## Level 10 → 11

**Goal:** Find the password in `data.txt`, which is base64-encoded

**Approach:** `cat data.txt` showed a base64-looking string (ending in `==` padding). First attempt `base64 -data.txt` failed on flag syntax (missing space/dash before the filename caused it to be parsed as an option).

**Solution:** `base64 -d data.txt` — the `-d` flag decodes base64 input, revealing the plaintext password directly

**Takeaway:** `base64 -d` decodes base64-encoded data; recognizable by its character set and `=`/`==` padding at the end
