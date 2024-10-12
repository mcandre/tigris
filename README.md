# tigris: Kindle comic book archiver

# EXAMPLE

```
$ tigris 101

$ ls ~/Downloads/tigris
000.png
001.png
002.png
...
```

Adjust `101` to match desired frame count.

# DISCLAIMER

For personal archival purposes only.

# LICENSE

BSD-2-Clause

# RUNTIME REQUIREMENTS

* [git](https://git-scm.com/) 2.46.1+
* [Kindle](https://www.amazon.com/b?ie=UTF8&node=16571048011) 7.20+
* [macOS](https://www.apple.com/macos) 15+

## Recommended

* [Amphetamine](https://apps.apple.com/us/app/amphetamine/id937984704)
* [ImageMagick](https://imagemagick.org/)

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

# CONTRIBUTING

For more information on developing tigris itself, see [DEVELOPMENT.md](DEVELOPMENT.md).

# SEE ALSO

* [harmonica](https://github.com/mcandre/harmonica), a comic book repackager
