# BUILDTIME REQUIREMENTS

* [git](https://git-scm.com/) 2.46.1+
* [Kindle](https://www.amazon.com/b?ie=UTF8&node=16571048011) 7.20+
* [macOS](https://www.apple.com/macos) 15+

## Recommended

* [Amphetamine](https://apps.apple.com/us/app/amphetamine/id937984704)
* [ImageMagick](https://imagemagick.org/)

# INSTALL

(Adjust git forks, clone URLs, remotes, HEAD pointer, and/or local directory name as needed.)

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
