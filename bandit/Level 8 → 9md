## Level 8 → 9

**Goal:** Find the one line in `data.txt` that occurs exactly once — every other line appears more than once

**Approach:** No known pattern to grep for, since the challenge is about line frequency rather than content

**Solution:** `sort data.txt | uniq -u` — sorting brings duplicate lines adjacent, then `uniq -u` filters to only lines with no duplicates

**Takeaway:** `uniq` only detects duplicates that are adjacent, so it needs sorted input first; `sort | uniq -u` is a standard pattern for finding unique entries in unsorted data
