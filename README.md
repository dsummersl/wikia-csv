A mirror of the [wikia csv plugin](http://vim.wikia.com/wiki/Csv).

Add the following to your ~/.vimrc to support CSV and TSV type files
automatically:

    autocmd BufNewFile,BufRead *.csv setf csv
    autocmd BufNewFile,BufRead *.tsv setf csv
    autocmd BufNewFile,BufRead *.tsv Delimiter \t
    autocmd BufNewFile,BufRead *.tsv setlocal ts=20 sw=25

See the plugin page for usage.
