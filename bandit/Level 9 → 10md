## Level 9 → 10

**Goal:** Find a password in `data.txt`, a mostly-binary file — the password is one of a few human-readable strings, preceded by several `=` characters

**Approach:** Tried `sort data.txt | grep '='` first, which failed since `sort` doesn't extract readable text from binary data — it only reorders lines. Switched to `strings data.txt | grep '='`, which pulls printable character sequences out of binary content.

**Solution:** Output showed several `==========`-prefixed lines — two were decoy English words ("the", "password is"), one was a genuine random-character string: `B0s2khmbT9u0geKuOoVGW3JZKhndE3BG`, which was the actual password

**Takeaway:** `strings` extracts readable text from binary/non-text files, unlike `sort` which just reorders existing lines; when a challenge includes decoys, verify a candidate matches the expected format (random string) rather than taking the first match
