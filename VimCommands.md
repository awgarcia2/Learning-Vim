# Vim Commands

## Opening a file in Vim
To open a file in vim use the command:

```vim <file>```

This will open up file in the vim editor

## Vim Modes
Upon entering the editor you will be placed in command (or normal) mode. This means you will be unable to type any text into the file. There are a few other modes as stated below.

Vim has a few main modes:
- Command mode (normal mode)
- Insert mode
- Visual mode

When in command mode you can change into insert mode by pressing `i`. Once in insert mode you will be able to type like any other text editor. To return to command mode use the `esc` key. 

Now to save and exit your file make sure you are in command mode by pressing `esc`. Once there a few basic commands for exiting the file are as follows:
- `:q` quit
- `:w` save
- `:wq` save and exit
- `:q!` exit without saving
To perfom any of the above commands enter command mode, type in the command then press enter. 

The rest of this document will go into what commands are avaliable in each mode.

## Command Mode

In command mode you can set various settings that influence the enviornment. These commands use the `set` keyword. Below are some common ones.

-`:set number` - toggles on line numbers
-`:set nonumber` - toggles off line numbers
-`:set showcmd` - shows the last command entered in the bottom right.
-`:set wildmenu` - adds auto complete for commands when you press tab.
-`:set showmatch` - when your cursor over a []{}() the matching one is highlighted
-`:set hlsearch` - highlight words that match your search.
-`:set incsearch` - searches as characters are entered.
-`:set relativenumber` - turns on relative line numbering.
-`:set cursorline` - turns on a line that remains under the line your cursor is on.
  
