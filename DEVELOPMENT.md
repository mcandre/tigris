# BUILDTIME REQUIREMENTS

* [git](https://git-scm.com/) 2.46.1+
* [ImageMagick](https://imagemagick.org/) 7.1.1+
* [Kindle](https://www.amazon.com/b?ie=UTF8&node=16571048011) 7.20+
* [macOS](https://www.apple.com/macos) 15+
* [ShellCheck](https://www.shellcheck.net/) 0.8.0+
* [Go](https://go.dev/) 1.23.2+
* [Python](https://www.python.org/) 3.12.1+
* [Snyk](https://snyk.io/)
* Provision additional dev tools with `./install`

## Recommended

* [Amphetamine](https://apps.apple.com/us/app/amphetamine/id937984704)

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
