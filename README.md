# Mirage overlays

**This repository is deprecated and has been merged into
[`opam-overlays`](https://github.com/dune-universe/opam-overlays/tree/master/packages/zarith),
which is the only one you need to add now.**

`dune-universe/mirage-opam-overlays` was an opam repository containing all
package definitions of cross compilation ports of existing packages from the
main default repository that cannot be cross compiled.

It was meant to be used by the [`opam-monorepo`](https://github.com/ocamllabs/dune-universe)
tool to allow you to vendor your dependencies and cross compiler your entire project
using `dune` only.

Since June 2026, 
[`opam-overlays`](https://github.com/dune-universe/opam-overlays/tree/master/packages/zarith), requires all packages to be both buildable with dune and cross-compilable, hence superseding this repo.
