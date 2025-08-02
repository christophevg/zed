# My Zed Configuration

For years, [TextMate](https://github.com/textmate/textmate) was my trusted editor. However, due to its unmaintained status, I’ve tried switching to other editors like Atom, but unfortunately, Microsoft abandoned it in favor of VS Code, which I’m not interested in using. I genuinely desire a text-oriented flexible editor, since I'm a very text/terminal-based polyglot.

Recently, I stumbled upon [Zed](https://zed.dev) and, after installing it and merely 1.5 hours fiddling, I was hooked. It’s like “TextMate The Next Generation.” and apparently it's from the creators of Atom 😉

This repository contains my settings and more, which initially aim to replicate my TextMate experience as closely as possible to facilitate a smooth transition 😇

## Installation

Clone this repository in `~/.config/`:

```console
$ cd ~/.config
$ git clone https://github.com/christophevg/zed
```

To enable the [CSpell extension](https://github.com/mantou132/zed-cspell) support with the `cspell.json` configuration in this zed-specific configuration folder:

Ensure that cspell finds the configuration [link it to a location cspell can find it](https://github.com/mantou132/zed-cspell/issues/1#issuecomment-2881938172):

```console
$ cd ~/.config
$ ln -s zed/cspell.json .
```

Install the `nl-nl` dictionary

```console
npm install -g @cspell/dict-nl-nl
npm install -g cspell
cspell link add @cspell/dict-nl-nl
```
Execute zed command: `editor: restart language server`
