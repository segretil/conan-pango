[![Download](https://api.bintray.com/packages/bincrafters/public-conan/pango%3Abincrafters/images/download.svg) ](https://bintray.com/bincrafters/public-conan/pango%3Abincrafters/_latestVersion)
[![Build Status Travis](https://travis-ci.com/bincrafters/conan-pango.svg?branch=stable%2F1.44.7)](https://travis-ci.com/bincrafters/conan-pango)
[![Build Status AppVeyor](https://ci.appveyor.com/api/projects/status/github/bincrafters/conan-pango?branch=stable%2F1.44.7&svg=true)](https://ci.appveyor.com/project/bincrafters/conan-pango)

## Conan package recipe for [*pango*](https://www.pango.org/)

Internationalized text layout and rendering library

The packages generated with this **conanfile** can be found on [Bintray](https://bintray.com/bincrafters/public-conan/pango%3Abincrafters).


## Issues

If you wish to report an issue or make a request for a package, please do so here:

[Issues Tracker](https://github.com/bincrafters/community/issues)


## For Users

### Basic setup

    $ conan install pango/1.44.7@bincrafters/stable

### Project setup

If you handle multiple dependencies in your project is better to add a *conanfile.txt*

    [requires]
    pango/1.44.7@bincrafters/stable

    [generators]
    pkg_config

Complete the installation of requirements for your project running:

    $ mkdir build && cd build && conan install ..

Note: It is recommended that you run conan install from a build directory and not the root of the project directory.  This is because conan generates *conanbuildinfo* files specific to a single build configuration which by default comes from an autodetected default profile located in ~/.conan/profiles/default .  If you pass different build configuration options to conan install, it will generate different *conanbuildinfo* files.  Thus, they should not be added to the root of the project, nor committed to git.


## Build and package

The following command both runs all the steps of the conan file, and publishes the package to the local system cache.  This includes downloading dependencies from "build_requires" and "requires" , and then running the build() method.

    $ conan create . bincrafters/stable


### Available Options
| Option        | Default | Possible Values  |
| ------------- |:----------------- |:------------:|
| shared      | False |  [True, False] |
| fPIC      | True |  [True, False] |


## Add Remote

    $ conan remote add bincrafters "https://api.bintray.com/conan/bincrafters/public-conan"


## Conan Recipe License

NOTE: The conan recipe license applies only to the files of this recipe, which can be used to build and package pango.
It does *not* in any way apply or is related to the actual software being packaged.

[MIT](https://github.com/feliwir/conan-pango/blob/stable/1.44.7/LICENSE.md)
