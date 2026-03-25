# CONFIGURATION

We use CLI flags for configuration.

## tigris

`tigris [<frames>]` captures raw archival panels to `~/Downloads/tigris/`

Adjust the frames to match the number of pages in your comic book.

Example:

1. Launch ereader app.
2. Open a comic to its cover page.
3. Tile ereader to the left half of the display.
4. Launch a terminal emulator, such as `Terminal`.
5. Tile the terminal emulator to the right half of the display.
6. Run `tigris [<frames>]`.

## Tips

* To end a console command early, foreground the console emulator and press `Control + C`
* To end a run in the macOS Script Editor application, press `Command + Period` (`.`)
* Queue `tigris` command in console emulator, then adjust the cursor to minimize Kindle HUD artifacts before submitting the command with the Return (Enter) key
* Temporarily silence browser and other application notifications during scans
* Keep backups of `tigris/` images before altering images with `euphrates`

## euphrates

`euphrates` trims panel borders.

* `-o <directory>` customizes the output directory path, default `<source directory>/../euphrates/`
* `-l <amount>` trims pixels from the left, e.g. 104 (default 0)
* `-t <amount>` trims pixels from the top, e.g. 70 (default 0)
* `-r <amount>` trims pixels from the right, e.g. 103 (default 0)
* `-b <amount>` trims pixels from the bottom, e.g. 69420 (default 0)

Example:

```sh
euphrates
```

## zip

Use a compressor, such as Archive Utility or the `zip` CLI tool, to bundle the desired panels into DRM-free comic ebooks.

`zip -r <archive-path> <source-directory>` compresses directories recursively into an archive. For comic books, use an archive path extension like `.cbz`.

`unzip -tvl <archive-path>` lists ZIP format ebook contents.
