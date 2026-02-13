# Awesome CMake [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome) ⭐ 437,051 | 🐛 69 | 📅 2026-01-28 with stars

[<img src="https://rawgit.com/onqtam/awesome-cmake/master/cmake-logo.svg" align="right" width="100">](https://cmake.org/)

> A curated list of awesome [CMake](https://cmake.org/) scripts, modules, examples and others

Your contributions are highly welcome (first see [CONTRIBUTING.md](origin/CONTRIBUTING.md)).

There is another file [`NonModernCMake.md`](origin/NonModernCMake.md) with other links worth taking a look, but they use obsolete practices which are considered non-modern - like not using `target_*`-based dependency management - see [`#16`](https://github.com/onqtam/awesome-cmake/issues/16) ⭐ 5,346 | 🐛 4 | 📅 2025-12-15 and [`#42`](https://github.com/onqtam/awesome-cmake/pull/42) ⭐ 5,346 | 🐛 4 | 📅 2025-12-15 for more details.

## Contents

* [Community](#community)
* [Resources](#resources)
* [Package Management / Build Systems](#package-management--build-systems)
* [Modules](#modules)
* [Utility Scripts](#utility-scripts)
* [Toolchains](#toolchains)
* [Examples / Templates](#examples--templates)
* [Other](#other)

## Community

* [`#cmake` on Freenode](http://webchat.freenode.net/?channels=cmake)
* [`/r/cmake` on Reddit](https://www.reddit.com/r/cmake/)
* [`/r/cpp` on Reddit](https://www.reddit.com/r/cpp/)
* [Official Discourse Forum](https://discourse.cmake.org/)
* [Stack Overflow](http://stackoverflow.com/questions/tagged/cmake)

## Resources

* [Web Book](https://github.com/ruslo/CGold) ⭐ 534 | 🐛 25 | 📅 2023-06-05 - CGold: The Hitchhiker’s [Guide](https://cgold.readthedocs.io) to the CMake. [`[BSD2]`][BSD-2-Clause]
* [Modern CMake](https://github.com/toeb/moderncmake) ⭐ 242 | 🐛 2 | 🌐 CMake | 📅 2016-08-31 - Modern CMake **PDF** and samples by the creator of [cmakepp](https://github.com/toeb/cmakepp) ⭐ 446 | 🐛 40 | 🌐 CMake | 📅 2021-12-27. [`[MIT]`][MIT]
* [Lecture](https://www.youtube.com/watch?v=y7ndUhdQuU8) - More Modern CMake ([slides & examples](https://github.com/Bagira80/More-Modern-CMake) ⭐ 172 | 🐛 0 | 🌐 CMake | 📅 2020-02-11)- by Deniz Bahadir, Meeting C++ 2018.
* [Lecture](https://www.youtube.com/watch?v=y9kSr5enrSk) - Oh No! More Modern CMake ([slides](https://github.com/Bagira80/More-Modern-CMake/raw/master/OhNoMoreModernCMake.pdf) ⭐ 172 | 🐛 0 | 🌐 CMake | 📅 2020-02-11)- by Deniz Bahadir, Meeting C++ 2019.
* [Tutorial](https://github.com/Wigner-GPU-Lab/Teaching/tree/master/CMake) ⭐ 62 | 🐛 6 | 🌐 C++ | 📅 2022-01-15 - A step-by-step guide for understanding CMake.
* [Tutorial](https://github.com/schweitzer/modern-cmake-tutorial) ⭐ 32 | 🐛 0 | 🌐 CMake | 📅 2020-03-12 - Tutorial and Example on How to Properly Use Modern CMake.
* [Latest Documentation](https://cmake.org/cmake/help/latest/)
* [FAQ](https://gitlab.kitware.com/cmake/community/-/wikis/FAQ)
* [Wiki](https://gitlab.kitware.com/cmake/community/-/wikis/home)
* [Webinars](https://cmake.org/webinars/)
* [Tutorial](https://www.siliceum.com/en/blog/post/cmake_01_cmake-basics) - Modern CMake tutorials part1: CMake basics
* [Article](http://foonathan.net/blog/2016/03/03/cmake-install.html) - Easily supporting CMake install and find\_package().
* [Article](http://foonathan.net/blog/2016/07/07/cmake-dependency-handling.html) - Easy dependency management for C++ with CMake and Git.
* [Article](https://steveire.wordpress.com/2016/08/09/opt-in-header-only-libraries-with-cmake/) - Opt-in header-only libraries with CMake.
* [Article](https://rix0r.nl/blog/2015/08/13/cmake-guide/) - Ultimate Guide to Modern CMake.
* [Article](https://web.archive.org/web/20190116071957/http://voices.canonical.com/jussi.pakkanen/2013/03/26/a-list-of-common-cmake-antipatterns/) - A list of common CMake antipatterns (from 2013 but still relevant).
* [Article](http://preshing.com/20170511/how-to-build-a-cmake-based-project/) - How to Build a CMake-Based Project.
* [Article](http://preshing.com/20170522/learn-cmakes-scripting-language-in-15-minutes/) - Learn CMake's Scripting Language in 15 Minutes.
* [Article](http://aosabook.org/en/cmake.html) - The architecture of CMake.
* [Lecture](https://www.youtube.com/watch?v=bsXLMQ6WgIk) - Effective CMake - by Daniel Pfeifer, C++Now 2017.
* [Article](https://devblogs.nvidia.com/parallelforall/building-cuda-applications-cmake/) - Building Cross-Platform CUDA Applications with CMake.
* [Article + Lecture](https://steveire.wordpress.com/2017/11/05/embracing-modern-cmake/) - Embracing Modern CMake - by Stephen Kelly.
* [Lecture](https://www.youtube.com/watch?v=eC9-iRN2b04) - Modern CMake for Modular Design - by Mathieu Ropert, CppCon 2017.
* [Article](https://pabloariasal.github.io/2018/02/19/its-time-to-do-cmake-right/) - It's Time To Do CMake Right (one of the best articles about CMake).
* Articles - A series on CMake - by Martin Hořeňovský
  * [Basic CMake usage](https://codingnest.com/basic-cmake/).
  * [Basic CMake, part 2: libraries](https://codingnest.com/basic-cmake-part-2/).
* [Lecture](https://www.youtube.com/watch?v=jt3meXdP-QI) - Introduction to CMake - by Florent Castelli, C++ Sweden 2018.
* [Article](http://bastian.rieck.me/blog/posts/2018/cmake_tips/) - Some nice and accurate CMake tips.
* [Article](http://unclejimbo.github.io/2018/06/08/Modern-CMake-for-Library-Developers/) - Modern CMake for Library Developers.
* [Article](https://gist.github.com/mbinna/c61dbb39bca0e4fb7d1f73b0d66a4fd1) - Effective Modern CMake: a great summary of most good practices - by Manuel Binna.
* [Book](https://crascit.com/professional-cmake/) - Professional CMake: A Practical Guide (paid).
* [Book](https://leanpub.com/effective-cmake) - Effective CMake: Practical Advice to Write Better CMake (not fully written yet).
* [Web Book](https://cliutils.gitlab.io/modern-cmake/) - An Introduction to Modern CMake.
* [YouTube Series](https://vector-of-bool.github.io/2018/08/12/cmake-good.html) - How to CMake Good. [`[CC0-1.0]`][CC0-1.0]
* [Article](https://cristianadam.eu/20190223/modifying-the-default-cmake-build-types/) - Modifying the default CMake build types/flags, toolchains and patches - Oh my! - by Cristian Adam.

## Package Management / Build Systems

* [vcpkg](https://github.com/Microsoft/vcpkg) ⭐ 26,614 | 🐛 1,298 | 🌐 CMake | 📅 2026-02-13 - A tool to acquire and build C++ open source libraries. Uses CMake internally as a build script language. [`[MIT]`][MIT]
* [Ninja](https://github.com/ninja-build/ninja) ⭐ 12,688 | 🐛 397 | 🌐 C++ | 📅 2026-01-20 - Build system that differs from others in two major respects: it is designed to have its input files generated by a higher-level build system (like CMake), and it is designed to run builds as fast as possible. [`[APACHE2]`][APACHE2]
* [conan](https://github.com/conan-io/conan) ⭐ 9,224 | 🐛 774 | 🌐 Python | 📅 2026-02-12 - Conan C++ Package Manager, implemented in Python and has a CMake integration backend. [`[MIT]`][MIT]
* [cpm](https://github.com/TheLartians/CPM) ⭐ 3,897 | 🐛 156 | 🌐 CMake | 📅 2026-01-18 - A setup-free CMake + git dependency manager. [`[MIT]`][MIT]
* [hunter](https://github.com/ruslo/hunter) ⚠️ Archived - Cross-platform package manager for C++ (based on CMake ExternalProject). [`[BSD2]`][BSD-2-Clause]
* [cpm](https://github.com/iauns/cpm) ⭐ 750 | 🐛 14 | 🌐 CMake | 📅 2021-08-28 - C++ Package Manager based on CMake and Git. [`[MIT]`][MIT]
* [fips](https://github.com/floooh/fips) ⭐ 503 | 🐛 58 | 🌐 Python | 📅 2026-01-26 - High-level build system/dependency management for distributed, multi-platform C/C++ projects. [`[MIT]`][MIT]
* [cget](https://github.com/pfultz2/cget) ⭐ 462 | 🐛 51 | 🌐 Python | 📅 2024-04-19 - CMake package retrieval. This can be used to download and install CMake packages. [`[BOOST]`][BOOST]
* [pmm](https://github.com/AnotherFoxGuy/pmm) ⚠️ Archived - PMM is a module for CMake that manages... package managers. [`[MIT]`][MIT]
* [FetchDependency](https://github.com/jpetrie/fetch-dependency) ⭐ 3 | 🐛 2 | 🌐 CMake | 📅 2026-01-25 - Configuration-time retrieval, configuration and building of dependencies. [`[MIT]`][MIT]
* [cppan](https://cppan.org/) - C++ Archive Network - C++ Package Manager based on CMake, implemented in C++14. [`[APACHE2]`][APACHE2]

## Modules

* [cmake-modules](https://github.com/rpavlik/cmake-modules) ⭐ 1,063 | 🐛 19 | 🌐 CMake | 📅 2025-02-10 - [Ryan Pavlik](https://github.com/rpavlik)'s collection of CMake modules. There are a number of find modules, especially for virtual reality and physical simulation, some utility modules, and some patches or workarounds for CMake itself. [`[BOOST]`][BOOST]
* [cmake-modules](https://github.com/bilke/cmake-modules) ⭐ 585 | 🐛 29 | 🌐 CMake | 📅 2025-11-05 - This is a collection of additional CMake modules. Most of them are from Ryan Pavlik. [`[BOOST]`][BOOST]
* [Metabench](https://github.com/ldionne/metabench) ⭐ 188 | 🐛 12 | 🌐 CMake | 📅 2021-05-01 - CMake module for compile-time microbenchmarks. [`[BOOST]`][BOOST]
* [CMake](https://github.com/Eyescale/CMake) ⭐ 155 | 🐛 13 | 🌐 CMake | 📅 2023-12-05 - [Eyescale](https://github.com/Eyescale)'s common CMake modules. [`[BSD3]`][BSD-3-Clause]
* [extra-cmake-modules](https://github.com/KDE/extra-cmake-modules) ⭐ 149 | 🐛 0 | 🌐 CMake | 📅 2026-02-06 - [KDE](https://github.com/KDE)'s extra modules and scripts for CMake. [`[BSD3]`][BSD-3-Clause]
* [cgcmake](https://github.com/chadmv/cgcmake) ⭐ 131 | 🐛 1 | 🌐 CMake | 📅 2021-06-08 - CMake modules for common applications related to computer graphics. [`[MIT]`][MIT]
* [FindTBB](https://github.com/justusc/FindTBB) ⭐ 89 | 🐛 8 | 🌐 CMake | 📅 2018-03-22 - CMake find module for Intel Threading Building Blocks. [`[MIT]`][MIT]
* [cmake-modules](https://github.com/jedbrown/cmake-modules) ⭐ 87 | 🐛 11 | 🌐 CMake | 📅 2020-10-21 - CMake modules for some scientific libraries. [`[BSD2]`][BSD-2-Clause]
* [FindMathematica](https://github.com/sakra/FindMathematica) ⭐ 64 | 🐛 2 | 🌐 CMake | 📅 2025-08-08 - CMake module for Mathematica. [`[MIT]`][MIT]
* [YCM](https://github.com/robotology/ycm) ⭐ 59 | 🐛 50 | 🌐 CMake | 📅 2025-07-17 - Extra CMake Modules for [Yet Another Robot Platform](https://github.com/robotology/yarp) ⭐ 585 | 🐛 246 | 🌐 C++ | 📅 2026-02-07 and friends. [`[BSD3]`][BSD-3-Clause]
* [cmake-modules](https://github.com/hanjianwei/cmake-modules) ⭐ 31 | 🐛 0 | 🌐 CMake | 📅 2015-04-19 - [hanjianwei](https://github.com/hanjianwei)'s CMake module collection. [`[MIT]`][MIT]
* [FindICU.cmake](https://github.com/julp/FindICU.cmake) ⭐ 30 | 🐛 3 | 🌐 C | 📅 2017-01-07 - CMake module to find International Components for Unicode (ICU) Library. [`[BSD2]`][BSD-2-Clause]
* [FindIDL](https://github.com/apriorit/FindIDL) ⭐ 25 | 🐛 3 | 🌐 CMake | 📅 2024-10-02 - CMake module for building [IDL](https://docs.microsoft.com/en-us/windows/win32/midl/interface-definition-idl-file) files with MIDL and generating CLR DLL using [Tlbimp](https://docs.microsoft.com/en-us/dotnet/framework/tools/tlbimp-exe-type-library-importer). [`[MIT]`][MIT]
* [FindWiX](https://github.com/apriorit/FindWiX) ⭐ 18 | 🐛 0 | 🌐 CMake | 📅 2022-10-31 - CMake module for building [Windows Installer](https://en.wikipedia.org/wiki/Windows_Installer) packages with [WiX toolset](http://wixtoolset.org). [`[BSD3]`][BSD-3-Clause]
* [CMakeCM](https://github.com/AnotherFoxGuy/CMakeCM) ⭐ 2 | 🐛 2 | 🌐 CMake | 📅 2022-05-18 - CMake Community Modules. `[NO LICENSE]`
* [Oranges](https://github.com/benthevining/Oranges) - [Ben Vining](https://github.com/benthevining)'s library of CMake modules and toolchains [`[GPL]`][GPL]

## Utility Scripts

These provide a wide range of functionality - from dealing with compiler flags to using tools. Some also contain modules.

* [cotire](https://github.com/sakra/cotire) ⚠️ Archived - Cotire (compile time reducer) is a CMake module that speeds up the build process of CMake based build systems by fully automating techniques as precompiled headers and unity builds for C and C++. [`[MIT]`][MIT]
* [cmakepp](https://github.com/toeb/cmakepp) ⭐ 446 | 🐛 40 | 🌐 CMake | 📅 2021-12-27 - Enhancement Suite for the CMake Build System. [`[MIT]`][MIT]
* [DownloadProject](https://github.com/Crascit/DownloadProject) ⚠️ Archived - CMake module for downloading an external project's source at configure time. [`[MIT]`][MIT]
* [sanitizers-cmake](https://github.com/arsenm/sanitizers-cmake) ⭐ 408 | 🐛 13 | 🌐 CMake | 📅 2025-11-04 - CMake module to enable sanitizers for binary targets. [`[MIT]`][MIT]
* [ucm](https://github.com/onqtam/ucm) ⭐ 213 | 🐛 4 | 🌐 CMake | 📅 2023-03-13 - For managing compiler/linker flags, collecting sources, precompiled headers, unity builds and others. [`[MIT]`][MIT]
* [cmake-precompiled-header](https://github.com/larsch/cmake-precompiled-header) ⭐ 159 | 🐛 19 | 🌐 CMake | 📅 2019-11-01 - Visual Studio and GCC precompiled header macro. [`[LICENSE]`](https://github.com/larsch/cmake-precompiled-header/blob/master/PrecompiledHeader.cmake#L31) ⭐ 159 | 🐛 19 | 🌐 CMake | 📅 2019-11-01
* [CMakePCHCompiler](https://github.com/nanoant/CMakePCHCompiler) ⭐ 103 | 🐛 9 | 🌐 CMake | 📅 2019-10-26 - CMake precompiled headers via custom compiler extension - with reuse support! [`[MIT]`][MIT]
* [ixm](https://github.com/slurps-mad-rips/ixm) ⚠️ Archived - Make CMake less painful when trying to write Modern Flexible CMake.  [`[MIT]`][MIT]
* [sugar](https://github.com/ruslo/sugar) ⚠️ Archived - CMake tools and examples: collecting source files, warnings suppression, etc. [`[BSD2]`][BSD-2-Clause]
* [CMake-codecov](https://github.com/RWTH-ELP/CMake-codecov) ⭐ 96 | 🐛 10 | 🌐 CMake | 📅 2025-05-05 - Enables code coverage and generates coverage reports with CMake targets. [`[GPL]`][GPL]
* [coveralls-cmake](https://github.com/JoakimSoderberg/coveralls-cmake) ⭐ 87 | 🐛 7 | 🌐 CMake | 📅 2020-02-26 - Coveralls JSON coverage generator and uploader for CMake. [`[MIT]`][MIT]
* [compatibility](https://github.com/foonathan/compatibility) ⚠️ Archived - Improved version of cmake-compile-features. [`[LICENSE]`](https://github.com/foonathan/compatibility/blob/master/LICENSE) ⚠️ Archived
* [cmake-get](https://github.com/pfultz2/cmake-get) ⭐ 63 | 🐛 3 | 🌐 CMake | 📅 2019-01-18 - Get dependencies in config or script mode. `[NO LICENSE]`
* [cmake-modules](https://github.com/Tronic/cmake-modules) ⭐ 45 | 🐛 1 | 🌐 CMake | 📅 2022-11-04 - LibFindMacros development repository and other cool CMake stuff. [`[LICENSE]`](https://github.com/Tronic/cmake-modules/blob/master/LibFindMacros.cmake#L2) ⭐ 45 | 🐛 1 | 🌐 CMake | 📅 2022-11-04
* [GreatCMakeCookOff](https://github.com/UCL/GreatCMakeCookOff) ⭐ 44 | 🐛 16 | 🌐 CMake | 📅 2023-06-07 - This is a repository of useful and less than useful CMake recipes. [`[MIT]`][MIT]
* [cmake-unit](https://github.com/polysquare/cmake-unit) ⭐ 38 | 🐛 4 | 🌐 CMake | 📅 2017-05-31 - Unit testing framework for CMake. [`[MIT]`][MIT]
* [buildem](https://github.com/janelia-flyem/buildem) ⚠️ Archived - Modular CMake-based system that leverages ExternalProject to simplify builds. [`[LICENSE]`](https://github.com/janelia-flyem/buildem/blob/master/LICENSE.txt) ⚠️ Archived
* [cppcheck-target-cmake](https://github.com/polysquare/cppcheck-target-cmake) ⭐ 18 | 🐛 0 | 🌐 CMake | 📅 2016-05-30 - Per-target CPPCheck for CMake. [`[MIT]`][MIT]
* [clang-tidy-target-cmake](https://github.com/polysquare/clang-tidy-target-cmake) ⭐ 16 | 🐛 0 | 🌐 CMake | 📅 2016-05-31 - Add clang-tidy checks to a target using CMake. [`[MIT]`][MIT]
* [iwyu-target-cmake](https://github.com/polysquare/iwyu-target-cmake) ⭐ 10 | 🐛 0 | 🌐 CMake | 📅 2016-05-30 - CMake integration for include-what-you-use. [`[MIT]`][MIT]
* [cmake-header-language](https://github.com/polysquare/cmake-header-language) ⭐ 4 | 🐛 0 | 🌐 CMake | 📅 2016-05-26 - CMake macro to determine the language of a header file. [`[MIT]`][MIT]
* [tooling-cmake-util](https://github.com/polysquare/tooling-cmake-util) ⭐ 3 | 🐛 0 | 🌐 CMake | 📅 2016-05-30 - Utility and common library for all polysquare CMake tools. [`[MIT]`][MIT]
* [fetch\_paths.cmake](https://github.com/XiaoLey/fetch_paths.cmake) ⭐ 0 | 🐛 0 | 🌐 CMake | 📅 2025-04-11 - Lightweight utility to simplify file/directory path retrieval in CMake, supporting dynamic searches and flexible output formats. [`[MIT]`](https://github.com/XiaoLey/fetch_paths.cmake/blob/main/LICENSE) ⭐ 0 | 🐛 0 | 🌐 CMake | 📅 2025-04-11
* [CMakeCooking](https://github.com/hakuch/CMakeCooking) - Flexible development environments for CMake projects with external dependencies
  . [`[APACHE2]`][APACHE2]

## Toolchains

* [dockcross](https://github.com/dockcross/dockcross) ⭐ 3,556 | 🐛 10 | 🌐 CMake | 📅 2026-02-03 - Cross compiling toolchains in Docker images. [`[MIT]`][MIT]
* [android-cmake](https://github.com/taka-no-me/android-cmake) ⭐ 1,230 | 🐛 45 | 🌐 CMake | 📅 2018-02-16 - CMake toolchain file and other scripts for the Android NDK. [`[BSD3]`][BSD-3-Clause]
* [polly](https://github.com/ruslo/polly) ⚠️ Archived - Collection of CMake toolchain files and scripts for cross-platform build and CI testing. [`[BSD2]`][BSD-2-Clause]
* [ios-cmake](https://github.com/cristeab/ios-cmake) ⭐ 317 | 🐛 1 | 🌐 CMake | 📅 2020-09-02 - Toolchain file and examples using CMake for iOS development. [`[BSD3]`][BSD-3-Clause]
* [qt-android-cmake](https://github.com/LaurentGomila/qt-android-cmake) ⭐ 249 | 🐛 4 | 🌐 CMake | 📅 2022-05-09 - For building and deploying Qt based apps on Android without QtCreator. [`[LICENSE]`](https://github.com/LaurentGomila/qt-android-cmake/blob/master/license.txt) ⭐ 249 | 🐛 4 | 🌐 CMake | 📅 2022-05-09
* [cmake-avr](https://github.com/mkleemann/cmake-avr) ⭐ 184 | 🐛 9 | 🌐 CMake | 📅 2022-04-17 - CMake toolchain for AVR. [`[LICENSE]`](https://github.com/mkleemann/cmake-avr/blob/master/LICENSE) ⭐ 184 | 🐛 9 | 🌐 CMake | 📅 2022-04-17
* [Arduino-CMake-Toolchain](https://github.com/a9183756-gh/Arduino-CMake-Toolchain) ⭐ 147 | 🐛 24 | 🌐 CMake | 📅 2023-02-24 - CMake toolchain for all official and 3rd party Arduino platforms. [`[MIT]`][MIT]
* [toolchains](https://github.com/mosra/toolchains) ⭐ 95 | 🐛 2 | 🌐 CMake | 📅 2025-10-15 - For cross-compiling with CMake. They are meant to be mainly used on ArchLinux. `[NO LICENSE]`
* [arduino-cmake](https://github.com/francoiscampbell/arduino-cmake) ⭐ 61 | 🐛 7 | 🌐 CMake | 📅 2021-01-11 - This is the CMake project settings for the Arduino platform. [`[MPL]`][MPL]
* [cmake](https://github.com/staticlibs/cmake/tree/master/toolchains) ⭐ 11 | 🐛 0 | 🌐 CMake | 📅 2019-05-09 - Collection of CMake toolchain files, mostly for static linking. [`[APACHE2]`][APACHE2]
* [mingw-w64-cmake](https://github.com/lachs0r/mingw-w64-cmake) - CMake-based MinGW-w64 Cross Toolchain - to build Windows binaries of mpv. [`[ISC]`][ISC]

## Examples / Templates

* [cmake-examples](https://github.com/ttroy50/cmake-examples) ⭐ 13,065 | 🐛 31 | 🌐 CMake | 📅 2024-02-28 - Useful CMake examples in a tutorial format. [`[MIT]`][MIT]
* [ModernCppStarter](https://github.com/TheLartians/ModernCppStarter) ⭐ 5,302 | 🐛 26 | 🌐 CMake | 📅 2025-03-12 - A template for modern C++ projects using CMake, CI, code coverage, clang-format, reproducible dependency management, tests using [doctest](https://github.com/onqtam/doctest) ⭐ 6,616 | 🐛 166 | 🌐 C++ | 📅 2026-02-12 and much more. [`[UNLICENSE]`][UNLICENSE]
* [cmake-cookbook](https://github.com/dev-cafe/cmake-cookbook) ⭐ 2,843 | 🐛 28 | 🌐 C++ | 📅 2021-06-01 - A huge CMake cookbook full of recipes. [`[MIT]`][MIT]
* [pitchfork](https://github.com/vector-of-bool/pitchfork) ⭐ 1,230 | 🐛 41 | 🌐 C++ | 📅 2024-04-26 - A set of conventions for native C and C++ projects. [`[MIT]`][MIT]
* [cmake-examples](https://github.com/pr0g/cmake-examples) ⭐ 1,221 | 🐛 1 | 🌐 CMake | 📅 2025-02-22 - A collection of as simple as possible, modern CMake projects. [`[MIT]`][MIT]
* [cmake-init](https://github.com/cginternals/cmake-init) ⭐ 934 | 🐛 25 | 🌐 CMake | 📅 2025-04-14 - Template for reliable, cross-platform C++ project setup using CMake. [`[LICENSE]`](https://github.com/cginternals/cmake-init/blob/master/LICENSE) ⭐ 934 | 🐛 25 | 🌐 CMake | 📅 2025-04-14
* [modern-cmake-sample](https://github.com/pabloariasal/modern-cmake-sample) ⭐ 679 | 🐛 5 | 🌐 CMake | 📅 2021-03-18 - Best practices and proper usage of CMake by using targets. `[NO LICENSE]`
* [cpp-project](https://github.com/bsamseth/cpp-project) ⭐ 620 | 🐛 2 | 🌐 CMake | 📅 2023-09-19 - Boiler plate for C++ projects - tests, CI, coverage, docs. [`[UNLICENSE]`][UNLICENSE]
* [package-example](https://github.com/forexample/package-example) ⭐ 406 | 🐛 0 | 🌐 CMake | 📅 2021-06-30 - Config mode of find\_package (examples for [this](http://stackoverflow.com/questions/20746936/cmake-of-what-use-is-find-package-if-you-need-to-specify-cmake-module-path-an) Stack Overflow question). `[NO LICENSE]`
* [how-to-export-cpp-library](https://github.com/robotology/how-to-export-cpp-library) ⭐ 374 | 🐛 11 | 🌐 CMake | 📅 2021-01-13 - An OS-agnostic template project for exporting either shared, static or header-only C++ library, sporting ctest and CI support, written in plain CMake with line-by-line tutorial comments. [`[MIT]`][MIT]
* [cpp-boilerplate](https://github.com/Lectem/cpp-boilerplate) ⭐ 325 | 🐛 1 | 🌐 CMake | 📅 2025-08-06 - Template that aims to be a reference for modern CMake and CI. [`[MIT]`][MIT]
* [mini-cmake-qt](https://github.com/euler0/mini-cmake-qt) ⭐ 220 | 🐛 1 | 🌐 CMake | 📅 2025-08-05 - Minimal CMake template for Qt 5 projects. [`[LICENSE]`](https://github.com/euler0/mini-cmake-qt/blob/master/LICENSE) ⭐ 220 | 🐛 1 | 🌐 CMake | 📅 2025-08-05
* [minimal\_cmake\_example](https://github.com/krux02/minimal_cmake_example) ⭐ 210 | 🐛 2 | 🌐 CMake | 📅 2019-01-17 - Minimal CMake example, that covers dependencies and packaging. [`[CC0-1.0]`][CC0-1.0]
* [cmake-example](https://github.com/bast/cmake-example) ⭐ 142 | 🐛 1 | 🌐 CMake | 📅 2021-02-04 - Example project which demonstrates various CMake features. [`[BSD3]`][BSD-3-Clause]
* [cmake\_templates](https://github.com/acdemiralp/cmake_templates) ⭐ 125 | 🐛 1 | 🌐 C++ | 📅 2022-04-28 - Templates for creating C++ libraries and executables (including conan). `[NO LICENSE]`
* [cpp14-project-template](https://github.com/arnavb/cpp14-project-template) ⭐ 68 | 🐛 2 | 🌐 CMake | 📅 2018-09-12 - A C++14 template with CI, tests, code coverage, docs and static analysis integration. [`[CC0-1.0]`][CC0-1.0]
* [cpp-template](https://github.com/joshpeterson/cpp-template) ⭐ 53 | 🐛 0 | 🌐 Python | 📅 2022-05-30 - A template C++ repository, using CMake and Catch. `[NO LICENSE]`
* [cmake\_snippets](https://github.com/adishavit/cmake_snippets) ⭐ 52 | 🐛 3 | 📅 2019-07-11 - Short copy-pasteable CMake snippets. [`[BSD3]`][BSD-3-Clause]
* [hunter-simple](https://github.com/forexample/hunter-simple) ⭐ 51 | 🐛 1 | 🌐 CMake | 📅 2019-02-20 - Example of downloading/installing dependencies using [ruslo/hunter](https://github.com/ruslo/hunter) ⚠️ Archived package manager. [`[BSD2]`][BSD-2-Clause]
* [BASIS](https://github.com/cmake-basis/BASIS) ⭐ 49 | 🐛 130 | 🌐 C++ | 📅 2021-07-07 - CMake [BASIS](https://cmake-basis.github.io) makes it easy to create sharable software and libraries that work together. [`[BSD2]`][BSD-2-Clause]
* [CMakeInstallExample](https://github.com/DeveloperPaul123/CMakeInstallExample) ⭐ 38 | 🐛 0 | 🌐 CMake | 📅 2021-09-07 - Installation example for a C++ project (Windows) with Cmake. `[NO LICENSE]`
* [android-cmake](https://github.com/forexample/android-cmake) ⭐ 35 | 🐛 0 | 🌐 C++ | 📅 2016-12-25 - Examples of using [ruslo/hunter](https://github.com/ruslo/hunter) ⚠️ Archived package manager for an Android application. [`[BSD2]`][BSD-2-Clause]
* [SeeMake](https://github.com/MhmRhm/SeeMake) ⭐ 12 | 🐛 0 | 🌐 CMake | 📅 2025-12-03 - A feature-packed, ready-to-use CMake template with testing, static and dynamic checks, coverage reports, and more. [`[MIT]`][MIT]

## Other

* [scikit-build](https://github.com/scikit-build/scikit-build) ⭐ 528 | 🐛 191 | 🌐 Python | 📅 2026-02-09 - Improved build system generator for CPython C extensions. [`[MIT]`][MIT]
* [suitesparse-metis-for-windows](https://github.com/jlblancoc/suitesparse-metis-for-windows) ⭐ 466 | 🐛 2 | 🌐 C | 📅 2024-03-16 - CMake scripts for painless usage of SuiteSparse+METIS. [`[BSD3]`][BSD-3-Clause]
* [cmake-language-server](https://github.com/regen100/cmake-language-server) ⭐ 400 | 🐛 22 | 🌐 Python | 📅 2025-02-11 - CMake Language Server Protocol Implementation. [`[MIT]`][MIT]
* [catkin](https://github.com/ros/catkin) ⚠️ Archived - CMake-based build system that is used to build all packages in Robot Operating System (ROS). [`[BSD3]`][BSD-3-Clause]
* [osg-3rdparty-cmake](https://github.com/bjornblissing/osg-3rdparty-cmake) ⭐ 196 | 🐛 10 | 🌐 CMake | 📅 2023-01-12 - CMake scripts for building OpenSceneGraph third party libraries. `[MIXED LICENSE]`
* [autovala](https://github.com/rastersoft/autovala) ⚠️ Archived - Program that automatically generates CMake configuration files for your Vala project. [`[GPL]`][GPL]
* [cmake-lint](https://github.com/richq/cmake-lint) ⚠️ Archived - Check for coding style issues in CMake files. cmakelint requires Python. [`[APACHE2]`][APACHE2]
* [configure-cmake](https://github.com/nemequ/configure-cmake) ⭐ 87 | 🐛 1 | 📅 2017-06-08 - configure-cmake is an autotools-style configure script for CMake-based projects. [`[CC0-1.0]`][CC0-1.0]
* [cmake-checks-cache](https://github.com/cristianadam/cmake-checks-cache) ⭐ 85 | 🐛 2 | 🌐 CMake | 📅 2022-03-04 - CMake checks cache helper modules. [`[MIT]`][MIT]
* [cmake-maven-plugin](https://github.com/cmake-maven-project/cmake-maven-project) ⭐ 81 | 🐛 0 | 🌐 Java | 📅 2025-06-19 - CMake integration for Maven builds. [`[APACHE2]`][APACHE2]
* [node-cmake](https://github.com/cjntaylor/node-cmake) ⚠️ Archived - CMake-based build system for node.js native modules. [`[ISC]`][ISC]
* [cmakeprojectmanager2](https://github.com/h4tr3d/cmakeprojectmanager2) ⭐ 73 | 🐛 4 | 🌐 C++ | 📅 2025-03-10 - Enhanced CMake Project Manager plugin for Qt Creator. `[NO LICENSE]`
* [cmake-d](https://github.com/dcarp/cmake-d) ⭐ 66 | 🐛 4 | 🌐 CMake | 📅 2023-06-09 - CMake for D2. [`[MIT]`][MIT]
* [git-cmake-format](https://github.com/kbenzie/git-cmake-format) ⭐ 59 | 🐛 2 | 🌐 CMake | 📅 2017-10-24 - Integrate clang-format into your CMake project hosted in a git repository. [`[LICENSE]`](https://github.com/kbenzie/git-cmake-format/blob/master/license.txt) ⭐ 59 | 🐛 2 | 🌐 CMake | 📅 2017-10-24
* [cmake-font-lock](https://github.com/Lindydancer/cmake-font-lock) ⭐ 47 | 🐛 6 | 🌐 CMake | 📅 2024-04-18 - Advanced syntax coloring support for CMake scripts inside Emacs. [`[GPL]`][GPL]
* [autocmake](https://github.com/coderefinery/autocmake) ⭐ 43 | 🐛 38 | 🌐 CMake | 📅 2023-02-06 - Using a autocmake.yml file [Autocmake](http://autocmake.readthedocs.io/en/latest/) composes CMake building blocks into a CMake project and generates CMakeLists.txt as well as a setup script, which serves as a front-end to CMakeLists.txt. [`[BSD3]`][BSD-3-Clause]
* [SoCMake](https://github.com/HEP-SoC/SoCMake) ⭐ 35 | 🐛 27 | 🌐 CMake | 📅 2026-02-12 - CMake based build system for hardware (ASIC, FPGA) and System-on-Chip build automation. [`[LGPL]`][LGPL]
* [cmake-ast](https://github.com/polysquare/cmake-ast) ⭐ 32 | 🐛 8 | 🌐 Python | 📅 2022-04-13 - Python module to reduce a CMake file to an AST. [`[MIT]`][MIT]
* [cmake\_check](https://github.com/DaelDe/cmake_check) ⚠️ Archived - Static analysis (linter) for the CMake language (e.g. to enforce modern CMake rules). [`[MIT]`][MIT]
* [version-from-git](https://github.com/MhmRhm/version-from-git) ⭐ 6 | 🐛 0 | 🌐 CMake | 📅 2022-05-04 - Bake git information into your binary. [`[MIT]`][MIT]
* [UseLATEX](https://gitlab.kitware.com/kmorel/UseLATEX) - Collection of CMake macros to simplify building LaTeX files. [`[BSD3]`][BSD-3-Clause]

## License

This is released under the [**`Creative Commons Attribution 4.0 International`**](http://creativecommons.org/licenses/by/4.0/) License `(CC BY 4.0)`.

[ISC]: https://opensource.org/licenses/ISC

[GPL]: https://www.gnu.org/licenses/gpl-3.0.html

[GPL2]: https://www.gnu.org/licenses/old-licenses/gpl-2.0.html

[LGPL]: https://www.gnu.org/licenses/lgpl-3.0.en.html

[MIT]: https://opensource.org/licenses/MIT

[BOOST]: http://www.boost.org/LICENSE_1_0.txt

[BSD-2-Clause]: https://opensource.org/licenses/BSD-2-Clause

[BSD-3-Clause]: https://opensource.org/licenses/BSD-3-Clause

[APACHE2]: http://www.apache.org/licenses/LICENSE-2.0

[CC0-1.0]: https://creativecommons.org/publicdomain/zero/1.0/

[MPL]: https://www.mozilla.org/en-US/MPL/2.0/

[UNLICENSE]: https://unlicense.org/
