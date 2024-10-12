# tigris: Kindle comic book archiver

# EXAMPLE

```
$ tigris 101

$ ls ~/Downloads/tigris
frame-0.png
frame-1.png
frame-2.png
...
```

Adjust `101` to match desired frame count.

# DISCLAIMER

For personal archival purposes only.

# LICENSE

BSD-2-Clause

# REQUIREMENTS

* [Kindle](https://www.amazon.com/b?ie=UTF8&node=16571048011) 7.20+
* [macOS](https://www.apple.com/macos) 15+

## Recommended

* [Amphetamine](https://apps.apple.com/us/app/amphetamine/id937984704)
* [ImageMagick](https://imagemagick.org/)

# INSTALL

Add .../tigris/bin to `PATH`.

# UNINSTALL

Remove .../tigris/bin from `PATH`.

# PREREQUISITES

1. Launch a console emulator, e.g. Terminal.
2. Open desired Kindle book to starting page.
3. Select `Window` -> `Full Screen Tile` -> `Left of Screen`.
4. Select console emulator as the right tile.

# TIPS

* Queue `tigris` command in console emulator, then adjust the cursor to minimize Kindle HUD artifacts before submitting the command with the Return (Enter) key.
* Temporarily silence browser and other application notifications during scans.
* To end the script early, foreground the console emulator and press `Control + C`.
