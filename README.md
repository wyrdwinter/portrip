# Portrip

A mass downloader for portraits on [a certain Neverwinter Nights server](https://nwn.sinfar.net).

## Installation

This runs on *nix systems and maybe on Windows WSL. You'll need a recent version
of [SBCL](http://www.sbcl.org/) and [Quicklisp](https://www.quicklisp.org/beta/). The former can be 
installed via a distribution package manager (or something like Homebrew), while
the latter has its own installation instructions.

You'll probably also want to symlink to this in your local `$PATH`.

## Use

```bash
$ ./portrip
Portrip: A Sinfar portrait downloader
Usage: portrip [mandatory arguments] [optional arguments]

mandatory arguments
  --players=            one or more Neverwinter Nights player account names
                         * e.g. "Account" or "Account1;Account2;Account3"

optional arguments
  --characters=         downloads specific portraits attached to the account
                         * e.g. "Char1;Char2;Char3"
                         * downloads all portraits when left unspecified
                         * this argument is not accepted for multiple accounts
  --directory=          the destination directory for portraits
                         * defaults to current directory
                         * creates directories if needed

```

## Bugs

It's been a while since I wrote this. It may fail in certain use cases. If you
care to use it and encounter an issue, I'd appreciate a bug report.
