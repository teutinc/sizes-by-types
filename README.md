sizes-by-types
==============

Bash script to get the sizes of files by their types in a specified path.

Howto
-----

To use it just type something like:
```
/path/to/script/sizes-by-types .
```
It should output somethig like:
```
8       foo (2)
2910292 bar (123)
```
Meaning that there is two files with 'foo' extention having a total size of 8 kilobytes, and 123 files having bar extention for a total size of 2910292 kilobytes.

If a line like this ```12      OTHERS (3)``` is appended at the end of the results, it means that there is 3 files that does not have a regular extention, and the total of size for those files is 12 kilobytes.

For the script, a regular extention is something matching this regular expression:
```
\.[a-zA-Z0-9_-]*$
```

Options
-------
Options available are:
```
    -t or --type [type(s)]    -- specify the type(s) of files (types must be separated by :)
    -v or --verbose           -- verbose output
    -h or --human-readable    -- display size in human readable format
    -k or --kilobytes         -- display size in kilobytes
    -s or --sort              -- sort the results by their sizes (ascendingly)
    -r or --reverse-sort      -- reverse sort
    --help                    -- print help
    --version                 -- print version
```


TODO
----
- Manage some options like:
```
     -i|--ignore-case -> ignore cases for extensions
     -e|--exclude -> reverse of type option
```
