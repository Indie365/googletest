# GoogleTest

#### OSS Builds Status:

[![Build Status](https://api.travis-ci.org/google/googletest.svg?branch=master)](https://travis-ci.org/google/googletest)
[![Build status](https://ci.appveyor.com/api/projects/status/4o38plt0xbo1ubc8/branch/master?svg=true)](https://ci.appveyor.com/project/GoogleTestAppVeyor/googletest/branch/master)

### Announcements:

#### Release 1.10.x

[Release 1.10.x](https://github.com/google/googletest/releases/tag/release-1.10.0)
is now available.

#### Coming Soon

*   Post 1.10.x googletest will follow
    [Abseil Live at Head philosophy](https://abseil.io/about/philosophy)
*   We are also planning to take a dependency on
    [Abseil](https://github.com/abseil/abseil-cpp).

## Welcome to **GoogleTest**, Google's C++ test framework!

This repository is a merger of the formerly separate GoogleTest and GoogleMock
projects. These were so closely related that it makes sense to maintain and
release them together.

### Getting started:

The information for **GoogleTest** is available in the
[GoogleTest Primer](googletest/docs/primer.md) documentation.

**GoogleMock** is an extension to GoogleTest for writing and using C++ mock
classes. See the separate [GoogleMock documentation](googlemock/README.md).

More detailed documentation for googletest is in its interior
[googletest/README.md](googletest/README.md) file.

## Features

*   An [xUnit](https://en.wikipedia.org/wiki/XUnit) test framework.
*   Test discovery.
*   A rich set of assertions.
*   User-defined assertions.
*   Death tests.
*   Fatal and non-fatal failures.
*   Value-parameterized tests.
*   Type-parameterized tests.
*   Various options for running the tests.
*   XML test report generation.

## Platforms

GoogleTest has been used on a variety of platforms:

*   Linux
*   Mac OS X
*   Windows
*   Cygwin
*   MinGW
*   Windows Mobile
*   Symbian
*   PlatformIO

## Who Is Using GoogleTest?

In addition to many internal projects at Google, GoogleTest is also used by the
following notable projects:

*   The [Chromium projects](http://www.chromium.org/) (behind the Chrome browser
    and Chrome OS).
*   The [LLVM](http://llvm.org/) compiler.
*   [Protocol Buffers](https://github.com/google/protobuf), Google's data
    interchange format.
*   The [OpenCV](http://opencv.org/) computer vision library.

## Related Open Source Projects

[GTest Runner](https://github.com/nholthaus/gtest-runner) is a Qt5 based
automated test-runner and Graphical User Interface with powerful features for
Windows and Linux platforms.

[GoogleTest UI](https://github.com/ospector/gtest-gbar) is a test runner that
runs your test binary, allows you to track its progress via a progress bar, and
displays a list of test failures. Clicking on one shows failure text. Google
Test UI is written in C#.

[GTest TAP Listener](https://github.com/kinow/gtest-tap-listener) is an event
listener for GoogleTest that implements the
[TAP protocol](https://en.wikipedia.org/wiki/Test_Anything_Protocol) for test
result output. If your test runner understands TAP, you may find it useful.

[gtest-parallel](https://github.com/google/gtest-parallel) is a test runner that
runs tests from your binary in parallel to provide significant speed-up.

[GoogleTest Adapter](https://marketplace.visualstudio.com/items?itemName=DavidSchuldenfrei.gtest-adapter)
is a VS Code extension allowing to view GoogleTest in a tree view, and run/debug
your tests.

[C++ TestMate](https://github.com/matepek/vscode-catch2-test-adapter) is a VS
Code extension allowing to view GoogleTest in a tree view, and run/debug your
tests.

[Cornichon](https://pypi.org/project/cornichon/) is a small Gherkin DSL parser
that generates stub code for GoogleTest.

## Requirements

GoogleTest is designed to have fairly minimal requirements to build and use with
your projects, but there are some. If you notice any problems on your platform,
please file an issue on the
[GoogleTest GitHub Issue Tracker](https://github.com/google/googletest/issues).

Patches for fixing them are welcome!

### Build Requirements

These are the base requirements to build and use GoogleTest from a source
package:

*   [Bazel](https://bazel.build/) or [CMake](https://cmake.org/). NOTE: Bazel is
    the build system that GoogleTest is using internally and tests against.
    CMake is community-supported.

*   A C++11-standard-compliant compiler

*   Windows, or a POSIX compliant system.

    Compilers on Cygwin do not enable POSIX compliance by default, leading to
    errors about missing functions such as `strdup()`, even though the
    standard libraries provide them. Pass e.g. the `-D_GNU_SOURCE` define to
    enable these functions.

## Contributing change

Please read the [`CONTRIBUTING.md`](CONTRIBUTING.md) for details on how to
contribute to this project.

Happy testing!
