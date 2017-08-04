* [dropEst](https://github.com/hms-dbmi/dropEst)
    * Must install `install.packages(c("Rcpp","RcppArmadillo", "RInside", "Matrix", "fitdistrplus"))` in R and check if `R.home()` path is same as you specify to cmake
```
CMake Error at /home/linuxbrew/.linuxbrew/Cellar/cmake/3.8.1/share/cmake/Modules/FindPackageHandleStandardArgs.cmake:137 (message):
  Could NOT find R (missing: RCPP_ARM_INCLUDE_DIR)
Call Stack (most recent call first):
  /home/linuxbrew/.linuxbrew/Cellar/cmake/3.8.1/share/cmake/Modules/FindPackageHandleStandardArgs.cmake:377 (_FPHSA_FAILURE_MESSAGE)
  CMake/FindR.cmake:117 (find_package_handle_standard_args)
  CMakeLists.txt:26 (find_package)
```
