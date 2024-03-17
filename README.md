# syms-web
syms-web is a single executable binary file that run  sympy codes via web browser (as like as MATLAB/Octave symbolic package codes)

syms-web is portable lightweight complex equation solver and calculator, And doesn't need to any required software to be installed for working, Just download and use it quickly. For example download `syms-aarch64` to fresh Termux and use it without any required software installation as explained in `example1` directory.

### Some key features of syms-web:
* Free
* Open source
* Portable
* Offline
* Lightweight
* Simple
* Quick
* Easy source code
* Handheld (run on smartphone)
* Strong symbolic package 
* Support Python codes
* Infinite process timeout 

# usage
Download a release and change files permission to executable, Then run:
`./syms`

The syms-web always run sympy codes which user input via browser at address `http://127.0.0.1:8080`.

# build
Run `build.sh` at source directory.

# releases 

V1:
`syms-aarch64` is compiled dynamically with `nuitka --standalone` command at python 3.11
