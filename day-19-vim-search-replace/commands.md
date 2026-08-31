# Day 19: Vim Navigation & Search/Replace

1. **gg / G** — jumps you straight to the top or bottom of the file. `gg` goes to line one, `G` goes to the last line. No scrolling required.

2. **:10 (go to line)** — types a line number after the colon and Vim takes you there instantly. Handy in long config files.

3. **/ (search forward)** — searches for a pattern moving down through the file. Type `/` followed by whatever you're hunting for, then hit Enter.

4. **? (search backward)** — same idea as `/`, just searching upward instead. Useful when you know the thing you want is above your cursor, not below it.

5. **n / N** — jumps to the next or previous match after a search. `n` repeats the search direction, `N` reverses it. Small keys, big time-saver.

6. **:%s/old/new/g** — Vim's find-and-replace. The `%` means the whole file, and the `g` means every match on each line, not just the first one.

7. **dw** — deletes from the cursor to the start of the next word. Faster than holding backspace.

8. **x** — deletes a single character under the cursor. The smallest edit Vim offers.

9. **o / O** — opens a new line and drops you into insert mode automatically. `o` opens below the current line, `O` opens above it.

10. **ZZ** — saves and quits in one motion, no colon required. Basically a shortcut for `:wq`.
