# syms-web
syms-web is a single executable binary file that run  sympy codes via web browser (as like as MATLAB/Octave symbolic package codes)

syms-web is portable lightweight complex equation solver and calculator, And doesn't need to any required software to be installed for working, Just download and use it quickly. For example download `syms-aarch64` to fresh Termux and use it without any required software installation as explained in `example1` directory.

Note: In sum cases such as complex integral equations with imaginary part as below code, The `sympy` module is lacking! Use `MATLAB`, `Octave`, `Wolfram Mathematica` instead.
```
x = symbols('x', real=True)
f = Integral(exp(-1j*x)/x, (x, 1, oo))
result = f.evalf()
print(result)
```

Equal MATLAB/Octave code:
```
pkg load symbolic
syms x;
f = int(exp(-1i*x)/x, x, 1, Inf);
result = double(f);
disp(result);
```

### Some key features of syms-web:
* Free
* Open source
* Portable
* User friendly web interface 
* Offline
* Lightweight
* Simple
* Quick
* Few source code lines
* Handheld (run on smartphone)
* Powerful symbolic package 
* Support Python codes
* Infinite process timeout 

# usage
Download a release and change files permission to executable, Then run:
`./syms`

The syms-web always run sympy codes which user input via browser at address `http://127.0.0.1:8080`.

# build
Run `build.sh` at source directory.

# releases 
V3:

* Rewritten with `tornado` module instead of `pywebio` module
* MathJax rendering of LaTeX expressions
* Simple and fast interactive web style 

V2:

* Improved performance
* Enhanced view

V1:

* `syms-aarch64` is compiled dynamically with `nuitka --standalone` command at python 3.11
