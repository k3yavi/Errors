* [Salmon](https://github.com/COMBINE-lab/salmon)
    * Two possible cases: Either boost installed with clang salmon is being installed with gcc or vice-versa
    * Second: boost has not been installed with c++11 flag.
```
[100%] Linking CXX executable salmon
../../external/install/lib/libstaden-read.a(libstaden_read_la-open_trace_file.o): In function `find_file_url':
open_trace_file.c:(.text+0xd26): warning: the use of `tempnam' is dangerous, better use `mkstemp'
/home/FILESERVER5/proteomics/tss38/anaconda3/lib/libboost_regex.a(icu.o): In function `boost::icu_regex_traits::isctype(int, unsigned long) const':
icu.cpp:(.text+0x166): undefined reference to `u_charType_54'
icu.cpp:(.text+0x213): undefined reference to `u_isblank_54'
icu.cpp:(.text+0x241): undefined reference to `u_isspace_54'
icu.cpp:(.text+0x325): undefined reference to `u_isspace_54'
icu.cpp:(.text+0x348): undefined reference to `u_digit_54'
```

* [Salmon](https://github.com/COMBINE-lab/salmon)
    * Had old build of Salmon but changed gcc after that.
    * Must delete external folder too since some of the older dependencies have been compiled using previous compiler.
