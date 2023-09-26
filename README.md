## WARNING: This is not maintained, does not work well and for now I consider is a failed experiment. However it's informative so I keep it around as reference. Do not use it if you don't know what you are doing.#

Common Build Configurations for `build2` 
=======================================

This repository provides **commonly used build configuration descriptions for `build2`** users. For example: "debug" and "release" configs for MSVC, Clang and GCC toolchains.

If you are familiar with CMake, those configuration files are equivalent to toolchain files in CMake, in addition to the default configuration modes provided by it.

Currently [`build2` does not provide yet any default ***high-level configurations*** like "debug" or "release" although it is in the plans](https://github.com/build2/build2/issues/11). Meanwhile this repository provides `build2` users a quick way to get the common set of build configurations ready without having to re-write them all the time.

This is also the starting point for gathering data on a potential future integration into `build2` itself (or at least [help the effort to add default configurations by default into `build2`](https://github.com/build2/build2/issues/11)).

## This is a Work In Progress

At this point it is too early to stabilize how this repository will be used so **we recommend to not yet use this with non-toy or non-prototype projects**.
For example, we are not sure at all about the file naming, organisation or usage patterns to recommend etc.

If you have suggestions, feel free to create new tickets to this project so we can discuss them.

# Usage

Before creating a configuration:

1. Acquire the config files you need from this repository (through copy or git-submodule)
2. Add `config.config.load=<path/to/config-file>` to your build configuration creation command (either `bdep init -C ...` or `bdep config create ..` or `bpk create ...`)
    - Note that you can still add other config variables and files to override or add to the ones set in the configs. For example if you use `config.config.load=clang-debug.build` but you want specifically to use `clang-10++` instead of whatever version `clang++`, add `config.cxx=clang-10++` to that command line to override that variable. To add to a variable use `+=` to append, `=+` to prepend.


# Development

This repository is tested by the CI of ADD-OTHER-PROJECT-HERE-WITH-A-LINK

Check ./TODO.md for a list of things missing and/or that need some thoughts.

