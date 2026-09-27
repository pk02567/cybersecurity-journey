## Level 7 → 8

**Goal:** Find the password in `data.txt`, on the line containing the word "millionth"

**Approach:** Several early attempts failed on file path — tried `/data.txt` (wrong, file wasn't at filesystem root) and a couple of malformed grep invocations with stray arguments

**Solution:** `grep 'millionth' data.txt` (file in the current home directory) returned the matching line directly, with the password as the second field

**Takeaway:** `grep 'pattern' filename` searches file contents for a matching line — much faster than opening/reading the whole file manually when you know what to search for
