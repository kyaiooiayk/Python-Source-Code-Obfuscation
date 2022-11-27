# Python-Source-Code-Obfuscation
Python Source Code Obfuscation
***

## Introduction
In software development, obfuscation creates Source Code that cannot be read by human. Reasons for doing so are:
  - To protect intellectual property
  - To protect trade secrets
  - To prevent reverse engineering a proprietary software program.
***

## Available options
- [pyarmor](https://pypi.org/project/pyarmor/) - It provides full obfuscation with hex-encoding; apparently doesn’t allow partial obfuscation of variable/function names only.
- [python-minifier](https://pypi.org/project/python-minifier/) — It minifies the code and obfuscates function/variable names. 
- [pyminifier](https://pypi.org/project/pyminifier/) - It does a good job in obfuscating names of functions, variables, literals; can also perform hex-encoding (compression) similar as pyarmor. Problem: after obfuscation the code may contain syntax errors and not run.
- [cython](https://cython.org/) - Cython is an optimising static compiler that takes your .py modules and translates them to high-performant C files. Resulting C files can be compiled into native binary libraries with no effort. When the compilation is done there’s no way to reverse compiled libraries back to readable Python source code. What distinguishes this option from the other is that the main reason for using cython is to make your code run faster rather than obfuscating it.

## References
- [Python source code obfuscation](https://medium.com/geekculture/python-source-code-obfuscation-6b97f88a460d)
***

