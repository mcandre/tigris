# BUILDTIME REQUIREMENTS

* a UNIX-like environment (e.g. [WSL](https://learn.microsoft.com/en-us/windows/wsl/))
* [bash](https://www.gnu.org/software/bash/) 4+
* [git](https://git-scm.com/) 2.46.1+
* [ImageMagick](https://imagemagick.org/) 7.1.1+
* [Kindle](https://www.amazon.com/b?ie=UTF8&node=16571048011) 7.20+
* [macOS](https://www.apple.com/macos) 15+
* [ShellCheck](https://www.shellcheck.net/) 0.10.0+
* [Go](https://go.dev/) 1.25.3+
* [Python](https://www.python.org/) 3.13.7+
* [Snyk](https://snyk.io/)
* Provision additional dev tools with `./install`

## Recommended

* [Amphetamine](https://apps.apple.com/us/app/amphetamine/id937984704)
* [zip](https://infozip.sourceforge.net/)

# AUDIT

```console
$ ./build audit
```

# LINT

```console
$ ./build lint
```

# TEST

```console
$ ./build [unit_test]
```
