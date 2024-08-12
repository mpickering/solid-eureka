Recompilation bug in cabal-install

* `cabal build exe:b` -- Observe failure
* Modify `pkgs.project` to add b
* `cabal build exe:b` -- Observe failure
* Modify `cabal.project` by adding a newline
* `cabal build exe:b` -- Observe success

