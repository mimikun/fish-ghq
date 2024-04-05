# fish-ghq

keybinding for [ghq]

## Requirements

* Install [ghq]
* Install [fzf], [fzy], [peco], [percol] or [skim]
* Install [fisher]

## Install

```fish
fisher install mimikun/fish-ghq
```

## Keybinding

* Ctrl-g: repository finder using [fzf], [fzy], [peco], [percol] or [skim].

## Variables

### `GHQ_SELECTOR`

Default selector is `fzf`. If you want to change selector, run

```fish
set -x GHQ_SELECTOR peco
# or
set -x GHQ_SELECTOR fzf
set -x GHQ_SELECTOR fzf-tmux
set -x GHQ_SELECTOR fzy
set -x GHQ_SELECTOR percol
set -x GHQ_SELECTOR sk
```

### `GHQ_SELECTOR_OPTS`

```fish
# fzf example
set -x GHQ_SELECTOR_OPTS "--no-sort --reverse --ansi --color bg+:13,hl:3,pointer:7"
# peco example
set -x GHQ_SELECTOR_OPTS "--layout=top-down --prompt='ghq>'"
```

## License

fish-ghq is MIT licensed. See [LICENSE](LICENSE.txt) file for details.

[ghq]:https://github.com/x-motemen/ghq
[peco]:https://github.com/peco/peco
[fzf]:https://github.com/junegunn/fzf
[fzy]:https://github.com/jhawthorn/fzy
[percol]:https://github.com/mooz/percol
[skim]:https://github.com/lotabout/skim
[fisher]:https://github.com/jorgebucaran/fisher
