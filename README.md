# ModMerge

Merge require blocks in `go.mod` files as [`go mod tidy` doesn't do it because reasons](https://github.com/golang/go/issues/56471).

I hacked this tool together in less than 2 hours and unsurprisingly there are a few drawbacks with this:

- `require` blocks come last after using this. Can be fixed with little effort I think?
- Comments in `require` blocks are not preserved.