# Emacs Editor
Emacs, originally named EMACS, is a family of text editors that are characterized by their extensibility. The manual for the most widely used variant, GNU Emacs, describes it as "the extensible, customizable, self-documenting, real-time display editor"
## Shortcut Keys Used

- C = Control Key
- M = Meta Key (Alt on PCs, Option on Macs)

Examples:

- C-a = Hold control, press 'a'.
- C-x o = Hold control, press 'x', release both, press 'o' (oh, not zero).

## Basics

| Keys | Description |
| --- | --- |
| C-x C-c | Quit Emacs. |
| C-g | Cancel any in progress keybinding/shortcut command. |
| C-x C-s | Save current buffer. |
| C-x b | Switch to a different buffer. |
| C-x k | Kill/close current buffer. |
| C-x C-f | Open a file. |
| C-/ | Undo the last action. |

## Movement

In addition to the arrow keys, these keybindings allow for cursor movements.

### Buffer/File

| Keys | Description |
| --- | --- |
| M-< | Move to beginning of buffer/file. |
| M-> | Move to end of buffer/file. |
| C-v | Move one screen forward. |
| M-v | Move one screen backward. |
| C-l | Center screen on position at cursor. |

### Lines

| Keys | Description |
| --- | --- |
| C-a | Move to beginning of line. |
| C-e | Move to end of line. |
| C-n | Move to the next line. |
| C-p | Move to the previous line. |
| M-g g | Go to line. |

### Words

| Keys | Description |
| --- | --- |
| M-f | Move forward one word. |
| M-b | Move backward one word. |

### Characters

| Keys | Description |
| --- | --- |
| C-f | Move forward one character. |
| C-b | Move backward one character. |

## Searching

| Keys | Description |
| --- | --- |
| C-s | Regex search for text in current buffer and move to it. Press C-s again to move to next match. |
| C-r | Same as C-s, but search in reverse. |
| M-% | Search and replace. |

## Kill Ring (Copy/Cut/Paste)

| Keys | Description |
| --- | --- |
| C-spacebar | Create a region (select). Use movement keys to expand the region selected. Then use copy/cut commands below. |
| M-w | Copy region to kill ring (copy). |
| C-w | Kill region (cut). |
| C-y | Yank (paste). |
| M-y | Cycle through kill ring after yanking/pasting. This is like a copy/paste clipboard. |
| M-d | Kill/delete word starting at cursor (cut). |
| C-k | Kill/delete line starting at cursor (cut). |

## Editing

| Keys | Description |
| --- | --- |
| Tab | Indent line. |
| C-j | New line and indent, equivalent to enter followed by tab. |
| M-\ | Delete all spaces and tabs around point. |
| C-d | Delete the next character. |
| M-backspace | Delete previous word. |
| C-x space (use movement keys to select up/down).C-x r t (type key to insert, then Enter) | Rectangle mode |

## Formatting Tricks

| Keys | Description |
| --- | --- |
| C-t | Swap two characters at the point/cursor. |
| M-u | Change the word at the point/cursor to uppercase. |
| M-l | Change the word at the point/cursor to lowercase. |
| C-u n char | Insert 'n' (a number) copies of 'char' (a character). |

## Help

| Keys | Description |
| --- | --- |
| C-h k key-binding | Describe the function bound to the key binding. To get this to work, you actually perform the key sequence after typing C-h k. |
| C-h f | Describe function. |

## Windows and Frame

| Keys | Description |
| --- | --- |
| C-x o | Switch cursor to another window. |
| C-x 1 | Delete all other windows, leaving only the current window in the frame. This doesn’t close your buffers, and it won’t cause you to lose any work. |
| C-x 2 | Split frame above and below. |
| C-x 3 | Split frame side by side. |
| C-x 0 | Delete current window. |

## Plugin: Cider

### Clojure Files

| Keys | Description |
| --- | --- |
| C-c M-n M-n | Switch to namespace of current buffer. |
| C-x C-e | Evaluate expression immediately preceding point. |
| C-c C-k | Compile current buffer/file. |
| C-c C-d C-d | Display documentation for symbol under point. |
| M-. and M-, | Navigate to source code for symbol under point and return to your original buffer. |
| C-c C-d C-a | Apropros search; find arbitrary text across function names and documentation. |

### REPL

| Keys | Description |
| --- | --- |
| M-x cider-jack-in | Start a REPL. |
| C-c C-x C-j C-j | Alternative to start a REPL. |
| C-↑, C-↓ | Cycle through REPL history. |
| C-enter | Close parentheses and evaluate. |

## Plugin: Paredit

| Keys | Description |
| --- | --- |
| M-x paredit-mode | Toggle paredit mode. |
| M-( | Surround expression after point in parentheses (paredit-wrap-round). |
| C-→ | Slurp; move closing parenthesis to the right to include next expression. |
| C-← | Barf; move closing parenthesis to the left to exclude last expression. |
| C-M-f, C-M-b | Move to the opening/closing parenthesis. |