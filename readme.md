# mdwc

by Phillip Alday

```
wc wrapper for pandoc MarkDown files with YAML block.

arguments:
  --title, -t    run wc on title line in initial YAML block
                 (note: will not work on multiline titles)
  --body, -b     run wc on body (everything after initial YAML block)

wc arguments supported: (see man wc for more details)
  --bytes, -c
  --chars, -m
  --words, -w
  --lines, -l
  --max-line-length, -L
  --files0-from

Default is wc on just the body (useful for situations with length limits such
as abstracts)
```
