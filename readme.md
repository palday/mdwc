# mdwc

by Phillip Alday

Available through my [`mead` tap](https://github.com/palday/homebrew-mead) for [Homebrew](https://brew.sh/) and [Linuxbrew](https://linuxbrew.sh/)


```
wc wrapper for pandoc MarkDown files with YAML block.

arguments:
  --title, -t            run wc on title line in initial YAML block
                         (note: will not work on multiline titles)

  --body,  -b            run wc on body (everything after initial YAML block)

  --field, -f            run wc on specified top-level YAML field
                         Note: this will extract multiline fields and can be
                         used to extract multliline titles. This method is
                         slower, which may be come apparant when applied to
                         large (numbers of) files.

  --key,   -k            synonym for --field. One of these may be removed
                         in the future

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
