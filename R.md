* [sake](https://github.com/naikai/sake)
    * [Check this](https://github.com/Homebrew/homebrew-science/issues/5730), The problem is R has been complied with gcc which by default does not install libgfortran.
    * Copy pasting `/usr/local/lib/gcc/6/libgcc_s.1.dylib` from `/usr/local/Cellar/gcc/6.3.0_1/lib/gcc/6/libgcc_s.1.dylib` as in the example below helped solved the issue.
```
Error in dyn.load(file, DLLpath = DLLpath, ...) :
  unable to load shared object '/usr/local/lib/R/3.4/site-library/minqa/libs/minqa.so':
  dlopen(/usr/local/lib/R/3.4/site-library/minqa/libs/minqa.so, 6): Library not loaded: /usr/local/lib/gcc/6/libgcc_s.1.dylib
  Referenced from: /usr/local/opt/gcc/lib/gcc/6/libgfortran.3.dylib
  Reason: image not found
ERROR: lazy loading failed for package ‘car’
```
