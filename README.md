# Mirage overlays

`dune-universe/mirage-opam-overlays` is an opam repository containing all
package definitions of cross compilation ports of existing packages from the
main default repository that cannot be cross compiled.

It's meant to be used by the [`opam-monorepo`](https://github.com/ocamllabs/dune-universe)
tool to allow you to vendor your dependencies and cross compiler your entire project
using `dune` only.

All packages' versions in this repository are suffixed with a `+mirage` to
distinguish them from the upstream variants. That means that the
`opam-overlays` port of package `abc` version `X.Y.Z` is available on this repo
as `abc` version `X.Y.Z+mirage`.
Note that if a cross compilation port is based on a dune port from
`dune-universe/opam-overlays`, for instance on the dune port of `abc.X.Y.Z`,
versioned `abc.X.Y.Z+dune`, the cross compilation port should be versioned
`abc.X.Y.Z+dune+mirage`.
