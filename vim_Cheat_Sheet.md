# Vim Cheat Sheet
 

Vim as main modes: Normal, Insert, and Visual:

- Normal mode is for navigation and commands.
- Insert mode is for text input. Use `i` to enter this mode.
- Visual mode is for selecting and manipulating text. Use `v` to enter this mode.

> Use `esc` to exit both Insert and Visual mode 

------------
Commands 

- `:q` -> **Fecha um Ficheiro**
- `:q!` -> **Fecha um Ficheiro, sem guardar**
- `:wq` -> **Fecha um Ficheiro, e guarda**

- `r` -> **replace char**
- `x` -> **delete char**
- `dd` -> **delete line**
- `u` -> **undo**, `ctrl + r` -> **redo**

- `:nLinha` -> **Avanca para a linha "nLinha"**
- `o` -> **Insert line bellow**
- `w` -> **Go to next word**
- `b` -> **Go to last word**
- `yy` -> **Copy line**
- `p` -> **Paste line**
- `ct"char"` -> **Change until "char"**
- `I (shift + i)` -> **Insert in the begining of the line**
- `A (shift + a)` -> **Insert in the end of the line**
- `D (shift + d)` -> **Delete everything to the end of the line**
- `C (shift + c)` -> **Change everything to the end of the line**

- `G (shift + g)` -> **Go to the end of the file**
- `gg` -> **Go to the top of the file**
- `zz` -> **center the cursor in the middle of the terminal**

- `{` -> **Go up a block of code**
- `}` -> **Go down a block of code**
- `f` -> **Go to next occurrence of the character, placing your cursor on top of the character**
- `t` -> **Go to next occurrence of the character, placing your cursor right before the character searched**

- `:!Shell comand` por exemplo `:!gcc *.c` 


- `*`  -> **Search other instances of the word**
- `:%s/search/replace` -> **Search and Replace in Vim**
- `.`  -> **Repeats last command**


