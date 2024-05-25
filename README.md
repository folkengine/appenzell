[![Build and Test](https://github.com/devplaybooks/cpp_cmake_cpm/actions/workflows/CI.yml/badge.svg)](https://github.com/devplaybooks/cpp_cmake_cpm/actions/workflows/CI.yml)
[![License: Apache 2.0](https://img.shields.io/badge/license-Apache%202.0-blue?style=flat-square)](LICENSE-APACHE)

---

WIP

# Appenzell

noun - [ˈapn̩ˌt͡sɛl]

1. A command-line tool for driving OCPP Profiles through an OCPP 2.0 system.
2. The Swiss canton that existed 1403 to 1597 that is the location of the earliest known yodel, which happened in 1545. It is described as "the call of a cowherd from Appenzell." - [source](https://en.wikipedia.org/wiki/Yodeling#History_of_Alpine_yodeling)

# Setup

## ubuntu linux

```bash
$> sudo apt update && sudo apt install libsox-fmt-all libsoxr-dev
```

To test try:

```bash
$> play data/484841__astounded__yodel.wav
```

# C++ Dev Playbook with CPM.cmake

Includes:

* [ClangFormat](https://clang.llvm.org/docs/ClangFormat.html) config file
* [CPM.cmake](https://github.com/cpm-cmake/CPM.cmake)
* Niels Lohmann's [JSON for Modern C++](https://json.nlohmann.me/) - [github](https://github.com/nlohmann/json)
* [PortAudio](https://github.com/PortAudio/portaudio)
* [libsndfile](https://github.com/libsndfile/libsndfile)
