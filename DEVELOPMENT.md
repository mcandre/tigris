# DEVELOPMENT

We follow standard, `make` based commands for performing build operations.

# DEV ENVIRONMENT

## Prerequisites

* [macOS](https://www.apple.com/os/macos/) Tahoe+
* an ereader, such as [Kindle](https://www.amazon.com/b?ie=UTF8&node=16571048011)
* [bash](https://www.gnu.org/software/bash/) 4+
* [git](https://git-scm.com/)
* [Go](https://go.dev/)
* [ImageMagick](https://imagemagick.org/)
* [make](https://pubs.opengroup.org/onlinepubs/9799919799/utilities/make.html)
* [ShellCheck](https://www.shellcheck.net/) 0.11.0+
* Provision additional dev tools with `make -f install.mk`

## Recommended

* [Amphetamine](https://apps.apple.com/us/app/amphetamine/id937984704)
* [Homebrew](https://brew.sh/)
* [zip](https://infozip.sourceforge.net/)

## Postinstall

Register `"$HOME/src/github.com/mcandre/tigris/bin` to `PATH` environment variable.

# TASKS

We automate engineering tasks.

## Security Audit

```sh
make audit
```

## Lint

```sh
make
```
