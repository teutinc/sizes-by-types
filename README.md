sizes-by-types
==============

Bash script to get the sizes of files by their types in a specified path.

TODO
----
- Manage some options like:
    - -t|--type [type]
    - -v|--verbose -> verbose output
    - --version -> print version
    - -h|--human-readable -> print size in human readable format
    - -k|--kilobytes -> print size in kilobytes
    - -b|--bytes -> print size in bytes
    - -s|--sort -> sort the results by size (default is ascending sort, and by ext if no sort is specified)
    - -r|--reverse-sort -> reverse sort
- Add a prettier output format, like du with some padding.
- Maybe permit combination of parameters, for example -svh -> sorted, verbose and humand readable
