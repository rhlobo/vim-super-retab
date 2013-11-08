vim-super-retab
===============

Converts tabs to spaces, or spaces to tabs, and provides a "super retab"
command to convert only the whitespace used for indentation in programs.

This is a mirror of [VimTip1592][1]


### Commands

| Command      | Description                                                           |
| :----------- | --------------------------------------------------------------------: |
| Space2Tab    | Convert spaces to tabs, only in indents.                              |
| Tab2Space    | Convert tabs to spaces, only in indents.                              |
| RetabIndent  | Execute Space2Tab (if `expandtab` is set), or Tab2Space (otherwise).  |


### Features

- The commands allow an argument to specify the column width; if none is given, the `tabstop` setting is used.
- Redundant spaces in an indent are removed (in the above mapping, converting tabs to spaces will not change lines where there is a space before a tab in the indent).
- The search history is not changed (pressing n will do the same search it would have done before the conversion was performed).
- The cursor position is restored, although the column will be slightly wrong owing to the different number of characters in the indent.


 [1]: http://vim.wikia.com/wiki/VimTip1592
