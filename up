#!/bin/bash

# Install homebrew
which brew || /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"

# Install tools
brew install \
 autojump \
 fish \
 git \
 node \
 python \
 ruby \
 stow \
 vim
brew install --HEAD tmux

# Make fish the default shell

# Clone dotfiles
[ -d ~/.files ] ||  git clone https://github.com/spinningarrow/.files ~/.files

# Install dotfiles
pushd ~/.files
stow fish
stow git
stow tmux
stow vim
popd
