Dotfiles
========

This is a repository for bootstrapping my dotfiles with [Dotbot][dotbot].

Mainly based off [bppr/dotfiles](https://github.com/bppr/dotfiles) and [begriffs/haskell-vim-now](https://github.com/begriffs/haskell-vim-now)

To run, clone this repo and run `./install`

To install/update vim plugins, `:PlugInstall`/`:PlugUpdate` in vim

### Other setup:

* Install updates in AppStore
* Install [Chrome](https://www.google.com/chrome/)
* Install Slack from the AppStore
* Install [Homebrew](https://brew.sh/)
* [Set up ssh keys](https://help.github.com/articles/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent/)
* `brew cask install iterm2`
* `brew install vim`
* `brew install vcprompt`
* `brew install gpg-agent`
* Use zsh for my shell:
  * `brew install zsh`
  * `sudo dscl . -create /Users/$USER UserShell /usr/local/bin/zsh`
* Haskell tools:
  * `brew install stack`
  * `stack install hlint` (ALE needs this to be global right now)
  * `stack build --copy-compiler-tool hindent` (per project)
* Set up PGP:
  * Install [Keybase](https://keybase.io)
  * `brew install gpg`
  * `keybase pgp gen --multi`
  * `git config --global user.signingkey <key id>`
  * `keybase pgp export -q <key id> | pbcopy`
  * [Add to GitHub](https://github.com/settings/keys)

[dotbot]: https://github.com/anishathalye/dotbot
