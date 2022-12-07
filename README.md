# Python-Source-Code-Obfuscation
Python Source Code Obfuscation
***

## Introduction
In software development, obfuscation creates Source Code that cannot be read by human. Reasons for doing so are:
  - To protect intellectual property
  - To protect trade secrets
  - To prevent reverse engineering a proprietary software program.
***

## Hashing vs. Encryption vs. Encoding vs. Obfuscation
- **Encoding** transforms data into another format using a scheme that is publicly available so that it can easily be reversed. It does not require a key as the only thing required to decode it is the algorithm that was used to encode it. *Examples*: ASCII, Unicode, URL Encoding, Base64. Encoding is for maintaining data **usability** and can be reversed by employing the same algorithm that encoded the content, i.e. no key is used.
- **Encryption** transforms data into another format in such a way that only specific individual(s) can reverse the transformation. It uses a key, which is kept secret, in conjunction with the plaintext and the algorithm, in order to perform the encryption operation. As such, the ciphertext, algorithm, and key are all required to return to the plaintext. *Examples*: AES, Blowfish, RSA. Encryption is for maintaining data **confidentiality** and requires the use of a key (kept secret) in order to return to plaintext.
- **Hashing** serves the purpose of ensuring integrity, i.e. making it so that if something is changed you can know that it’s changed. Technically, hashing takes arbitrary input and produce a fixed-length string. *Examples*: SHA-3, MD5. Hashing is for validating the **integrity** of content by detecting all modification thereof via obvious changes to the hash output.
- **Obfuscation** makes something harder to understand. It’s important to note that obfuscation is not a strong control (like properly employed encryption) but rather an obstacle. It, like encoding, can often be reversed by using the same technique that obfuscated it. Obfuscation is used to **prevent** people from understanding the meaning of something.
***

## Available options
- [pyarmor](https://pypi.org/project/pyarmor/) - It provides full obfuscation with hex-encoding; apparently doesn’t allow partial obfuscation of variable/function names only.
- [python-minifier](https://pypi.org/project/python-minifier/) — It minifies the code and obfuscates function/variable names. 
- [pyminifier](https://pypi.org/project/pyminifier/) - It does a good job in obfuscating names of functions, variables, literals; can also perform hex-encoding (compression) similar as pyarmor. Problem: after obfuscation the code may contain syntax errors and not run.
- [cython](https://cython.org/) - Cython is an optimising static compiler that takes your .py modules and translates them to high-performant C files. Resulting C files can be compiled into native binary libraries with no effort. When the compilation is done there’s no way to reverse compiled libraries back to readable Python source code. What distinguishes this option from the other is that this can be used is to make your code run faster rather than obfuscating it.
***

## Available tutorials
- [How to cythonise your code](https://github.com/kyaiooiayk/High-Performance-Computing-in-Python/blob/master/tutorials/cythonizing/GitHub_MD_rendering/How%20to%20cythonize%20your%20code.ipynb)
***

## References
- [Python source code obfuscation](https://medium.com/geekculture/python-source-code-obfuscation-6b97f88a460d)
- [Hashing vs. Encryption vs. Encoding vs. Obfuscation](https://danielmiessler.com/study/encoding-encryption-hashing-obfuscation/)
***

