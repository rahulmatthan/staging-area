# staging-area

Temporary web hosting for HTML pages Rahul wants to show someone. Anything pushed to
`main` is served at **https://exmachina.in/staging-area/<slug>/** within a minute.
Public to anyone with the link, unlisted, meant to be taken down once seen.

```
stage up   <slug> <file-or-folder>   put a page up   (a file becomes <slug>/index.html)
stage down <slug>                    take it down
stage list                           what is up, and since when
```

`stage` lives in `bin/` and is symlinked into `~/.local/bin`. A folder is copied whole,
so relative `gifs/` and `stills/` paths keep working; a single `.html` file is copied
as `index.html`.
