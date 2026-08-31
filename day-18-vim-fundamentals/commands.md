#  Day 18: Vim Fundamentals

1. **vim <file>** — opens a file in Vim. If the file doesn't exist yet, Vim creates it the moment you save.

2. **i (insert mode)** — switches Vim from its default command mode into insert mode, which is the only mode where typing actually adds text to the file.

3. **Esc (command mode)** — exits insert mode and returns to command mode, where keystrokes are treated as commands rather than text. Nearly every Vim action starts by hitting this first.

4. **:w** — saves (writes) the file without closing Vim, letting you keep editing afterward.

5. **:q** — quits Vim. This only works cleanly if there are no unsaved changes.

6. **:wq / :x** — saves and quits in one step. `:x` behaves almost the same, except it only writes if the file was actually changed.

7. **:q!** — force-quits without saving, discarding any changes made since the last save. The `!` is what overrides Vim's normal refusal to quit with unsaved edits.

8. **dd** — deletes the entire current line. It also copies that line into Vim's internal buffer, so it can be pasted elsewhere.

9. **yy / p** — `yy` copies ("yanks") the current line without deleting it; `p` pastes whatever was last yanked or deleted, right after the cursor's current line.

10. **u / Ctrl+r** — `u` undoes the last change; `Ctrl+r` redoes a change that was just undone, in case you undid one step too many.
