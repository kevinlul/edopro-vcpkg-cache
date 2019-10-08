# EDOPro vcpkg binary cache

[EDOPro](https://github.com/edo9300/ygopro.git) builds against dependences from [vcpkg](https://github.com/microsoft/vcpkg.git) on Windows and Linux. Because vcpkg builds from source, this can take some time, slowing down build automation systems. This repo holds prebuilt `installed` folders, compressed, for Travis CI.

As required by EDOPro, binaries here are built on the x86-windows-static triplet, and to match Travis CI, with the MSVC v141 toolchain (Visual Studio 2017).

## Package contents

vcpkg name | portfile version | licence
--- | --- | ---
[bzip2](https://bzip2.sourceforge.io/) | 1.0.6-4 | BSD3-style 
[curl\[core,ssl,winssl\]](https://github.com/curl/curl) | 7.66.0 | MIT/X11-style
[discord-rpc](https://github.com/discordapp/discord-rpc) | 3.4.0 | MIT/Expat
[fmt](https://github.com/fmtlib/fmt) | 6.0.0 | MIT/Expat with binary exception
[libevent](https://github.com/libevent/libevent) | 2.1.11 | BSD3
[libflac](https://xiph.org/flac/index.html) | 1.3.2-6 | BSD3
[libgit2](https://github.com/libgit2/libgit2) | 0.28.3 | GPL2 with linking exception
[libjpeg-turbo](https://github.com/libjpeg-turbo/libjpeg-turbo) | 2.0.2 | BSD3-style
[libogg](https://xiph.org/ogg/) | 1.3.4 | BSD3
[libpng](https://github.com/glennrp/libpng) | 1.6.37-4 | BSD2-style
[libsndfile\[core,external-libs\]](https://github.com/erikd/libsndfile) | 1.0.29-8 | LGPL2.1
[libvorbis](https://xiph.org/vorbis/) | 1.3.6-9eadecc-3 | BSD3
[lua\[core,cpp\]](https://www.lua.org/download.html) | 5.3.5-2 | MIT/Expat
[mpg123](https://www.mpg123.de/) | 1.25.8-6 | LGPL2.1
[nlohmann-json](https://github.com/nlohmann/json) | 3.7.0 | MIT/Expat
[openal-soft](https://github.com/kcat/openal-soft) | 1.19.1-2 | LGPL2
[openssl-windows](https://github.com/openssl/openssl) | 1.0.2s-1 | Apache 2.0
openssl | 1 | Apache 2.0
[rapidjson](https://github.com/Tencent/rapidjson) | d87b698-1 | MIT/Expat
[sqlite3](https://www.sqlite.org/index.html) | 3.29.0-1 | public domain
[zlib](https://github.com/madler/zlib) | 1.2.11-5 | BSD2-style

vcpkg is licensed under the MIT/Expat licence.

## x64-linux (Bionic GCC7) package contents
vcpkg name | portfile version | licence
--- | --- | ---
[curl\[core,ssl,openssl\]](https://github.com/curl/curl) | 7.66.0 | MIT/X11-style
[discord-rpc](https://github.com/discordapp/discord-rpc) | 3.4.0 | MIT/Expat
[fmt](https://github.com/fmtlib/fmt) | 6.0.0 | MIT/Expat with binary exception
[libevent](https://github.com/libevent/libevent) | 2.1.11 | BSD3
[libflac](https://xiph.org/flac/index.html) | 1.3.2-6 | BSD3
[libgit2](https://github.com/libgit2/libgit2) | 0.28.3 | GPL2 with linking exception
[libogg](https://xiph.org/ogg/) | 1.3.4 | BSD3
[libsndfile\[core,external-libs\]](https://github.com/erikd/libsndfile) | 1.0.29-8 | LGPL2.1
[libvorbis](https://xiph.org/vorbis/) | 1.3.6-9eadecc-3 | BSD3
[lua\[core\]](https://www.lua.org/download.html) | 5.3.5-2 | MIT/Expat
[mpg123](https://www.mpg123.de/) | 1.25.8-6 | LGPL2.1
[nlohmann-json](https://github.com/nlohmann/json) | 3.7.0 | MIT/Expat
[openal-soft](https://github.com/kcat/openal-soft) | 1.19.1-2 | LGPL2
[openssl-unix](https://github.com/openssl/openssl) | 1.0.2s-1 | Apache 2.0
openssl | 1 | Apache 2.0
[rapidjson](https://github.com/Tencent/rapidjson) | d87b698-1 | MIT/Expat
[sqlite3](https://www.sqlite.org/index.html) | 3.29.0-1 | public domain
[zlib](https://github.com/madler/zlib) | 1.2.11-5 | BSD2-style

## dependencies-osx.7z
Contains two folders, libevent and irrlicht, containing their corresponding built binaries.
Built on macOS 10.14 against SDK 10.11 and targeting version 10.11.
