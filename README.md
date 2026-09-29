# code.waffle.systems

This repository serves the Go vanity import paths under `code.waffle.systems` through GitHub Pages.

The `go` command fetches `https://code.waffle.systems/<path>?go-get=1` and reads the `go-import` meta tag.
`404.html` is a copy of `index.html`, so every package path below a module returns the tag.
The `go` command reads the tag from a 404 response as well.

To add a module, add one `go-import` line (and optionally a `go-source` line) with the module's own prefix to both HTML files.
