
- [ ] find a better way to mix the tuplets elements
    - maybe just through includes?
    - one way would be to provide a lib+cliexe tool that generates the configs for the user...
        - if we go this direction, then using the libs internal to `build2` might help integration into it's distribution?
- [ ] add sanitizers (ASAN, TSAN, UBSAN, MSAN)
- [ ] add recommended warnings flags (see Jason Turner ones: https://github.com/cpp-best-practices/cppbestpractices/blob/master/02-Use_the_Tools_Available.md#compilers for a first set, see if there are other sets recommended)
- [ ] for now we assume all configs are for C or C++ toolchains, consider extending that (to rust? D?)

