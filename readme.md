bloc
===

`bloc` is a macOS utility for quickly blocking a website without leaving the comfort of your terminal.

![](bloc.gif)

Installation
===

Installing `bloc` is very easy: you just need to clone this very same repo at the latest release and then source the `bloc` file in your bash profile. Here's how I do it in my [dotfiles](https://github.com/mattmezza/dotfiles) (see plugins.sh and plugins.txt).

```bash
git clone git@github.com:mattmezza/bloc.git
```
Usage
===

What follows is the output of `bloc`, accessible at any time.

```
Usage:
    bloc [OPT] ARGS
OPT:
    -u|--unblock
    -h|--help
    -v|--version
ARGS:
    sub.domain.tld (e.g. twitter.com, or www.facebook.com)
Examples:
    $ bloc twitter.com        # blocks twitter.com
    $ bloc -u twitter.com     # unblocks twitter.com
```

Development
===

Developing `bloc` is quite easy. Clone the repo and start editing the `bloc` file.

