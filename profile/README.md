**this project has no afilliation with the [Zig Software Foundation](https://ziglang.org/).**

## zigbuild

This project contains `zig build` editions of various C/C++ packages.

We are particularly focused on using Zig as a build system for C/C++ packages, so this may not be a good reference point for all that the Zig language has to offer.

# Build philosophy

A few rules to keep in mind:

- Let Zig do the heavy lifting. The packages are only ever configured by a `build.zig` file, and may have had their original build processes nuked.

- If the package has dependencies, `build.zig.zon` is used in order to fetch them.
 
- Each package installs its headers to your build's include directory.
