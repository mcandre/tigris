# tigris & euphrates: comic book archival utilities

[![Lint](https://github.com/mcandre/tigris/actions/workflows/lint.yml/badge.svg)](https://github.com/mcandre/tigris/actions/workflows/lint.yml) [![license](https://img.shields.io/badge/license-BSD-0)](LICENSE.md)

# DISCLAIMER

For personal archival purposes only.

# SUMMARY

tigris helps to automate the painstaking task of archiving electronic comic books.

# EXAMPLE

Open Kindle to the start of your favorite comic book.

Use `Window` -> `Full Screen Tile` -> `Left of Screen` to tile Kindle into a left half-fullscreen orientation.

Then run our special archival utilities:

```console
% cd ~/Downloads

% tigris

% euphrates

% zip -r euphrates.cbz euphrates

% unzip -tvl euphrates.cbz
Archive:  euphrates.cbz
    testing: euphrates/   OK
    testing: euphrates/000.png   OK
    testing: euphrates/001.png   OK
    testing: euphrates/002.png   OK
...
```

# DOWNLOAD

```
git clone https://github.com/mcandre/tigris.git ~/src/github.com/mcandre/tigris
```

## Prerequisites

* [macOS](https://www.apple.com/os/macos/) Tahoe+
* an ereader, such as [Kindle](https://www.amazon.com/b?ie=UTF8&node=16571048011)
* [bash](https://www.gnu.org/software/bash/) 4+
* [git](https://git-scm.com/)
* [ImageMagick](https://imagemagick.org/#gsc.tab=0)

### Recommended

* [Amphetamine](https://apps.apple.com/us/app/amphetamine/id937984704)
* [Homebrew](https://brew.sh/)
* [zip](https://infozip.sourceforge.net/)

## Postinstall

Register `"$HOME/src/github.com/mcandre/tigris/bin` to `PATH` environment variable.

For details on tuning tigris & euphrates, see [CONFIGURATION](CONFIGURATION.md).

For details on building from source, see [DEVELOPMENT](DEVELOPMENT.md).

# RBAC

Warning: The first several runs of the application may trigger OS permission prompts, for the console emulator, Script Editor, and/or tigris.

Repeat until all permission prompts appear to be resolved:

1. Grant the permission to the respective application(s).
2. Quit and relaunch the terminal emulator.
3. Retry the operation.

Recommend prototyping archival scans with a small frame count (e.g. 3) in order to accelerate troubleshooting.

# RESOURCES

Prior art, personal plugs, and tools for managing digital content.

* [Comic Book Plus](https://comicbookplus.com/) - public domain comics
* [mcandre/buttery](https://github.com/mcandre/buttery) - an animated GIF editor
* [mcandre/harmonica](https://github.com/mcandre/harmonica) - a comic book repackager
* [mcandre/nile](https://github.com/mcandre/nile) - an ebook normalizer

🌾
