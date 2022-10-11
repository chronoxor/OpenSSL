# OpenSSL
OpenSSL 64-bit binaries for MinGW and Visual Studio

# Contents
  * [Features](#features)
  * [Requirements](#requirements)
  * [How to build?](#how-to-build)

# Features
* Supported compilers: MSYS2/Mingw-x64, Visual Studio 2022 (64-bit)
* Supported version: OpenSSL 1.1.1r
* Windows platform

# Requirements
* Windows
* [perl](https://strawberryperl.com)
* [MSYS2](https://www.msys2.org)
* [Visual Studio](https://www.visualstudio.com)

# How to build?

### Download OpenSSL archive
```shell
curl https://www.openssl.org/source/openssl-1.1.1r.tar.gz --output openssl-1.1.1r.tar.gz
```

### Extract OpenSSL sources
```shell
tar -xvzf openssl-1.1.1r.tar.gz
```

### Windows (MSYS2)
```shell
cd openssl-1.1.1r
perl Configure mingw64 no-shared
make
make install
```

### Windows (Visual Studio)
```shell
cd openssl-1.1.1r
perl Configure VC-WIN64A no-shared
nmake
nmake install
```
