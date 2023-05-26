# Basic Vi Commands
vi is a screen-oriented text editor originally created for the Unix operating system. The portable subset of the behavior of vi and programs based on it, and the ex editor language supported within these programs, is described by the Single Unix Specification and POSIX.
## Modes & Controls

| Command | Description |
| --- | --- |
| vi filename | Edit filename |
| vi -r filename | Edit last version of filename after crash |
| vi + n filename | Edit filename at end of file |
| vi + filename | Edit filename at end of file |
| vi +/str filename | Edit filename at first occurrence of str |

| Command | Description |
| --- | --- |
| :w | Save |
| :x or :wq | Save & Exit |
| :q | Exit if no changes made |
| :q! | Exit & discard any changes |

## Cursor Navigation

| Command | Description |
| --- | --- |
| h or ← | Cursor left |
| j or ↓ | Cursor down |
| k or ↑ | Cursor up |
| l or → | Cursor right |
| w | Next word |
| W | Next blank delimited word |
| b | Start of word |
| B | Start of blank delimited word |
| e | End of word |
| W | End of blank delimited word |
| ( | Back a sentence |
| ) | Forward a sentence |
| { | Back a paragraph |
| } | Forward a paragraph |
| 0 | Beginning of line |
| $ | End of line |
| 1G | Start of file |
| G | End of file |
| :n | nth line of file |
| f< char > | Forward to char |
| F< char > | Back to char |
| H | Top of screen |
| M | Middle of screen |
| L | Bottom of screen |
| % | Matching bracket |
| gg | Start of document |

## Inserting Text

| Command | Description |
| --- | --- |
| i | Insert before cursor |
| a | Append after cursor |
| I | Insert before line |
| A | Append after line |
| o | Add new line after current line |
| O | Add new line before current line |
| r | Overwrite one character |
| R | Overwrite many characters |
| :r file | Reads file and inserts it after this line |
| p | Put after the position or line |
| P | Put before the position or line |
| C | Rewrite the whole line |

## Marking Text (Visual Mode)

| Command | Description |
| --- | --- |
| v | Start visual mode, mark lines, then do command (such as y-yank) |
| V | Start Likewise visual mode |
| o | Move to other end of marked area |
| ctrl + v | Start visual block mode |
| O | Move to Other corner of block |
| aw | Mark a word |
| ab | A () block (with braces) |
| aB | A {} block (with brackets) |
| ib | Inner () block |
| iB | Inner {} block |
| esc | Exit visual mode |

## Visual commands

| Command | Description |
| --- | --- |
| > | Shift right |
| < | Shift left |
| y | Yank (copy) marked text |
| d | Delete marked text |
| ~ | Switch case |

## Cut and Paste

| Command | Description |
| --- | --- |
| yy | yank (copy) a line |
| 2yy | yank 2 lines |
| yw | yank word |
| y$ | yank to end of line |
| p | put (paste) the clipboard after cursor |
| P | put (paste) before cursor |
| dd | delete (cut) a line |
| dw | delete (cut) the current word |
| x | delete (cut) current character |

## Deleting Text

| Command | Description |
| --- | --- |
| x | Delete character to right of cursor |
| X | Delete character to left of cursor |
| D | Delete the rest of line |
| dd or :d | Delete current line |
| ndw | Deletes the next n words |
| ndb | Deletes the previous n words |
| ndd | Deletes n lines starting with current |
| :x,yd | Delete lines x through y |
| :r < file > | Reads file and inserts it after this line |
| d{nav_cmd} | Overwrite many characters |

## Searching

| Command | Description |
| --- | --- |
| /string | Search forward for string |
| ?string | Search backwards for string |
| n | Go to next match |
| N | Go to previous match |
| :set ic | Ignore case while searching |
| :set noic | Case-sensitive searching |
| :set nu | Turn on line numbers |
| :x,yg/str | Search for str from line x to line y |
| :g/str/cmd | Run cmd on lines containing str |
| * | Search for next instance of current word |
| # | Search for last instance of current word |
| :%s/old/new/g | Replace all old with new throughout file |
| :%s/old/new/gc | Replace all old with new throughout file with confirmations |

## Working with multiple files

| Command | Description |
| --- | --- |
| :e filename | Edit a file in a new buffer |
| :bnext (or :bn) | Go to next buffer |
| :bprev (of :bp) | Go to previous buffer |
| :bd | Delete a buffer (close a file) |
| :sp filename | Open a file in a new buffer and split window |
| ctrl + ws | Split windows |
| ctrl + ww | Switch between windows |
| ctrl + wq | Quit a window |
| ctrl + wv | Split windows vertically |

## Other

| Command | Description |
| --- | --- |
| u | Undo last change |
| J | Join lines |
| nJ | Join next n lines |
| . | Repeat last command |
| U | Undo all changes to line |
| ctrl + c | Escape insert mode |