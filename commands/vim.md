# VIM

- Insert Mode: `i` / Normal Mode: `ESC`.

- Navigation: LEFT (`h`), RIGHT (`l`), UP (`k`), DOWN (`j`)

- Navigating words: Start of next word (`w`), End of word (`e`), Beginning of word (`b`).

- Combine number with navigation. Eg: `3w` (move to beginning of 3rd word), `3l` (move right 3 times).

- Enter a sequence of text multiple times using the format: `<number>i<text>ESC`. Eg: `10 + i + hello + Esc` will enter hello 10 times.

- Use `%` (Shift + 5) to move the matching bracket.

- `0` move to the start of line, `$` (Shift + 4) move to end of line.

- `*` next / `#` previous occurance of words under the cursor.

- `gg` go to the beginning of file, `G` go the end of file. `<number>G` go to a specified line in the file. Eg: `10G` go to line 10.

- `/` + `<text>` search for text. Press enter and use `n` (to next term), `N` (to previous term).  

- `o` insert a line below current line, `O` insert a line above current line.

- `x` removes character under the cursor, `X` removes character before the cursor.

- `r` replace character under cursor.

- `d` delete. Eg: `dw` will delete the word towards right.

- `.` repeat the previous command.

- Use `v` to enter visual mode. Eg: press `v` select some words and press `d` to delete them.

- `:w` Save, `:q` Quite, `:q!` Quit without saving.

- `u` to undo, `Ctrl + R` to redo.
