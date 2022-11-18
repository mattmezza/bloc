bloc
===

`bloc` is a macOS utility for quickly blocking a website without leaving the comfort of your terminal.

![](bloc.gif)

`bloc` edits the `/etc/hosts` file, so it needs `sudo` privileges to run.

Installation
===

Installing `bloc` is very easy: you just need to clone this very same repo at the latest release and then source the `bloc` file in your bash profile. Here's how I do it in my [dotfiles](https://github.com/mattmezza/dotfiles) (see plugins.sh and plugins.txt).

```bash
git clone git@github.com:mattmezza/bloc.git && cd $_
./bloc twitter.com
```

Usage
===

Some examples:

- block twitter for 20 min: `bloc twitter.com && sleep 1200 && bloc -u twitter.com`
- block work websites: `cat work.txt | xargs -n1 bloc` where `work.txt` contains a multi-line list of domains
- block socials: `cat social.txt | while read -r i;do bloc $i; done`

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

