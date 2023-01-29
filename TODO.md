
- [ ] find a better way to mix the tuplets elements
    - maybe just through includes?
    - one way would be to provide a lib+cliexe tool that generates the configs for the user...
        - if we go this direction, then using the libs internal to `build2` might help integration into it's distribution?
        - also consider using a syntax like `build2` cli: `tool @config-mame -d config/location/ msvc,debug,asan,warnings-turner` (the last part being the sequence of common options we want) - that way it also makes the whole thing usable through `bdep config create ... config.hlconfig=windows,debug,asan,warnings-turner`
        - a way to list what are the options would be useful
        - an "interactive" way to do so would be too
        - consider using k-config?
        - this way would also allow some meta-configs, like "defaults" which would generate the usual configs for most toolchains (debug/release/asan?) or "all" etc. considering only the provided toolchains: `msvc` would mean `msvc,defaults` which would mean both `msvc,debug`, `msvc,debug,asan`, `msvc,release`, `msvc,release,asan` all at once
- [ ] add sanitizers
    - [x] ASAN (temptative..)
    - [ ] TSAN
    - [ ] UBSAN
    - [ ] MSAN
- [ ] add recommended warnings flags (see Jason Turner ones: https://github.com/cpp-best-practices/cppbestpractices/blob/master/02-Use_the_Tools_Available.md#compilers for a first set, see if there are other sets recommended)
- [ ] for now we assume all configs are for C or C++ toolchains, consider extending that (to rust? D?)

