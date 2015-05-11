# Overview

A mirror of the [wikia csv plugin](http://vim.wikia.com/wiki/Csv).

Add the following to your ~/.vimrc to support CSV and TSV type files
automatically:

    autocmd BufNewFile,BufRead *.csv setf csv
    autocmd BufNewFile,BufRead *.tsv setf csv
    autocmd BufNewFile,BufRead *.tsv Delimiter \t
    autocmd BufNewFile,BufRead *.tsv setlocal ts=20 sw=25

# Keys

Key | Mode | Description
--- | ---- | -----------
H | normal | Move left one column in the CSV.
J | normal | Move down one row in the CSV (stay in focused column).
K | normal | Move up one row in the CSV (stay in focused column).
L | normal | Move right one column in the CSV.
0 | normal | Move to the first column.
$ | normal | Move to the last column.
gm | normal | Jump back to focused column/row.

# Commands

Command | Description
------- | -----------
:Delimiter | Change the delimiter for a file. Takes a single character.
:DC | Delete the current column.
:SC | Search the current column.
:Csv # | Highlight a specific column (0 to turn off).
:HL # | Set the heading line number
:Sort | Sort by the current column. Can sort visually selected regions.
:CC | Copy the current column.
