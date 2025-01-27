## WineMaking

- `arch -x86_64 zsh`
- from https://brew.sh/
  - `/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)`
- from https://gitlab.winehq.org/wine/wine/-/wikis/MacOS-Building
  - `/usr/local/bin/brew install --formula bison mingw-w64 pkgconfig` and as requested:
    - `export PATH="/usr/local/opt/bison/bin:$PATH"`
  - `/usr/local/bin/brew install freetype gnutls molten-vk sdl2`
    - `export PKG_CONFIG_PATH=/usr/local/lib/pkgconfig`
- `/usr/local/bin/brew install ffmpeg gstreamer`
- `./configure.sh`
- `make -j12` build using 12 cores
- `./wine notepad`
