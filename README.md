# GNU C and C++ Alternatives

These scripts configure `update-alternatives` for GNU compilers
**gcc** and **g++**. Prior to running a script, the compiler versions
of interest, including the system's default version, should be
installed, and either define integer (only!) environment variables
**DEFAULT_COMPILER_VERSION** and **ALTERNATIVE_COMPILER_VERSIONS** or
edit their values at the top of script. If more than one version is
defined in **ALTERNATIVE_COMPILER_VERSIONS**, they should separated by
spaces.

Note that the script `debian-compiler-alternatives` removes the
alternatives group *cpp* and makes **cpp** a follower of **gcc**
instead.
