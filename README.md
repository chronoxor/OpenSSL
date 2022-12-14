# OpenSSL
OpenSSL 64-bit binaries for MinGW and Visual Studio

# Contents
  * [Features](#features)
  * [Requirements](#requirements)
  * [How to build?](#how-to-build)

# Features
* Supported compilers: MSYS2/Mingw-x64, Visual Studio 2022 (64-bit)
* Supported version: OpenSSL 3.0.7
* Windows platform

# Requirements
* Windows
* [perl](https://strawberryperl.com)
* [MSYS2](https://www.msys2.org)
* [Visual Studio](https://www.visualstudio.com)

# How to build?

### Download OpenSSL archive
```shell
curl https://www.openssl.org/source/openssl-3.0.7.tar.gz --output openssl-3.0.7.tar.gz
```

### Extract OpenSSL sources
```shell
tar -xvzf openssl-3.0.7.tar.gz
```

### Windows (MSYS2)
```shell
cd openssl-3.0.7
perl Configure mingw64 no-shared
make
make install
```

### Windows (Visual Studio)
```shell
cd openssl-3.0.7
perl Configure VC-WIN64A no-shared
nmake
nmake install
```
