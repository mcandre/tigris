# tigris & euphrates: (Kindle) comic book archival utilities

# EXAMPLE

Open Kindle to the start of your favorite comic book.

Use `Window` -> `Full Screen Tile` -> `Left of Screen` to tile Kindle into a left half-fullscreen orientation.

Then run our special archival utilities:

```
$ tigris

$ euphrates

$ zip -r ~/Downloads/euphrates.cbz ~/Downloads/euphrates

$ unzip -tvl ~/Downloads/euphrates.cbz
Archive:  ~/Downloads/euphrates.cbz
    testing: euphrates/   OK
    testing: euphrates/000.png   OK
    testing: euphrates/001.png   OK
    testing: euphrates/002.png  OK
...
```

# ABOUT

## tigris

`tigris [<frames>]` captures raw archival panels to `~/Downloads/tigris/`

Adjust the frames to match the number of pages in your comic book.

## euphrates

`euphrates` trims panel borders.

* `-n <frames>` controls the limit of images that euphrates processes
* `-o <directory>` customizes the output directory path, default `<source directory>/../euphrates/`
* `-l <amount>` trims pixels from the left, e.g. 104 (default 0)
* `-t <amount>` trims pixels from the top, e.g. 70 (default 0)
* `-r <amount>` trims pixels from the right, e.g. 103 (default 0)
* `-b <amount>` trims pixels from the bottom, e.g. 69420 (default 0)

See `euphrates -h` for more detail.

## zip

Use a compressor, such as Archive Utility or the `zip` CLI tool, to bundle the desired panels into DRM-free comic ebooks.

`zip -r <archive-path> <source-directory>` compresses directories recursively into an archive. For comic books, use an archive path extension like `.cbz`.

`unzip -tvl <archive-path>`

# DISCLAIMER

For personal archival purposes only.

# LICENSE

BSD-2-Clause

# RUNTIME REQUIREMENTS

* [git](https://git-scm.com/) 2.46.1+
* [ImageMagick](https://imagemagick.org/) 7.1.1+
* [Kindle](https://www.amazon.com/b?ie=UTF8&node=16571048011) 7.20+
* [macOS](https://www.apple.com/macos) 15+

## Recommended

* [Amphetamine](https://apps.apple.com/us/app/amphetamine/id937984704)
* [zip](https://linux.die.net/man/1/zip)

# INSTALL

1. Clone the project to a local directory.

```console
$ git clone https://github.com/mcandre/tigris.git ~/tigris
```

2. Add .../tigris/bin to `PATH`.

~/.zshrc:

```zsh
# ...
export PATH="$PATH:$HOME/tigris/bin"
```

# UNINSTALL

1. Remove .../tigris/bin from `PATH`.

~/.zshrc:

```zsh
# ...
```

2. Remove local clone directory.

```console
$ rm -rf ~/tigris
```

# APPLICATION PRIVILEGES

The first several runs of the application may trigger OS permission prompts, for the console emulator, Script Editor, and/or tigris.

Repeat until all permission prompts appear to be resolved:

1. Grant the permission to the respective application(s).
2. Quit and relaunch the console emulator.
3. Retry the tigris operation.

Recommend prototyping archival scans with a small frame count (e.g. 3) in order to accelerate troubleshooting.

# PREREQUISITES

1. Launch a console emulator, e.g. Terminal.
2. Open desired Kindle book to starting page.
3. Select `Window` -> `Full Screen Tile` -> `Left of Screen`.
4. Select console emulator as the right tile.

# TIPS

* To end the script early, foreground the console emulator and press `Control + C`.
* Queue `tigris` command in console emulator, then adjust the cursor to minimize Kindle HUD artifacts before submitting the command with the Return (Enter) key.
* Temporarily silence browser and other application notifications during scans.
* Keep backups of `tigris/` images before altering the images with `euphrates`.

# CONTRIBUTING

For more information on developing tigris itself, see [DEVELOPMENT.md](DEVELOPMENT.md).

# SEE ALSO

* [bao](https://github.com/mcandre/bao), a PDF compressor
* [buttery](https://github.com/mcandre/buttery), an animated GIF editor
* [harmonica](https://github.com/mcandre/harmonica), a comic book repackager
* [nile](https://github.com/mcandre/nile), an ebook normalizer
