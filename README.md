# hunter-foo

## motivation
I need platform-agnostic environment which provides a set of common C/C++ libs.
1. Windows build is a must.
2. Tools should also be available on OSX and Linux.
3. Complicated setup (Ex. cygwin or msys2 with its own package manager) should be avoided.
## tools
CMake - https://cmake.org/download/  
hunter - https://github.com/ruslo/hunter cpp package manager  
HunterGate.cmake - https://github.com/hunter-packages/gate CMake extension script  
cmder - http://cmder.net/ self-contained terminal emulator with minimal tooling (ls, tree, git, vim etc.)
# usage
You will need a quite new CMake installed and working cpp compiler. Then just do:

    export HUNTER_ROOT=<path>
    git clone <repo>
    sh ./build.sh
... and CMake will detect your environment, download/build external libraries under HUNTER_ROOT dir, create IDE or Makefile project under _build dir.

Enjoy!