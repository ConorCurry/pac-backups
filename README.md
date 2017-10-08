## Pacman package list for a new system install.

Organized into core packages and dependencies, to maintain
the package database structure for a new system.

Should be able to just install the core packages,
then check the installed dependencies against the
relevant file in this repository.

### pac-explicit.pkg

This contains all explicitly installed packages, from pacman repos. Install first.

### pac-foreign.pkg

This contains AUR packages. Install these with pacaur, second.

### pac-asdeps.pkg

Most of these should be installed as automatic depedencies of explicitly installed packages,
though might contain additional packages that were installed as optional dependencies.
Install this subset last with the --asdeps option.

TODO: make optional dependencies filtered out better, so that orphaned deps don't get installed.
