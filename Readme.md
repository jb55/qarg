
# qarg

Convert stdin to a single quoted argument

## Example

```bash
$ cabal install pointfree
$ echo -n "\\\f -> length . filter f" | qarg pointfree
(length .) . filter
```

## Use case

Handy for running commands like this from vim

```vim
V:!qarg pointfree
```

This will convert a visual selection to pointfree style
