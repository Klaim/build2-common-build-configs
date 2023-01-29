Common Build Configurations for `build2` 
=======================================

This repository provides **commonly used build configuration descriptions for `build2`** users. For example: "debug" and "release" configs for MSVC, Clang and GCC toolchains.

Currently [`build2` does not provide yet any default ***high-level configurations*** like "debug" or "release" although it is in the plans](https://github.com/build2/build2/issues/11). Meanwhile this repository provides `build2` users a quick way to get the common set of build configurations ready without having to re-write them all the time.

This is also the starting point for gathering data on a potential future integration into `build2` itself (or at least [help the effort to add default configurations by default into `build2`](https://github.com/build2/build2/issues/11)).

## This is a Work In Progress

At this point it is too early to stabilize how this repository will be used so **we recommend to not yet use this with non-toy or non-prototype projects**.
For example, we are not sure at all about the file naming, organisation or usage patterns to recommend etc.

If you have suggestions, feel free to create new tickets to this project so we can discuss them.

# Usage

When creating a configuration (through `bdep init -C ...` or `bdep config create ..` for example)



# Development

This repository is tested by the CI of ADD-OTHER-PROJECT-HERE-WITH-A-LINK


