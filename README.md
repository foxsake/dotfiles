This repository holds my configuration files so that I can clone them to other machines easily.

## Installation

Go to home directory and paste:

```bash
git clone https://github.com/foxsake/dotfiles ~/.dotfiles
```

### Vim

To install vim configurations, paste:
```bash
ln -s ~/.dotfiles/vim/vim ~/.vim 
ln -s ~/.dotfiles/vim/vimrc ~/.vimrc
```
To add vim plugins,
```bash
cd ~/.dotfiles/vim
git submodule add <plugin address> vim/bundle/<plugin name>
```
To install vim plugins, cd to your dotfiles directory then
```bash
git submodule init
git submodule update
```
or
```bash
git submodule update --init
```
#### Upgrading plugins
To upgrade a plugin bundle, go to the plugin directory and pull
```bash
git pull origin master
```
To upgrade all bundled plugins
```bash
git submodule foreach git pull origin master
```

### Tmux
To install tmux configurations, paste:
```bash
ln -s ~/.dotfiles/tmux/tmux.conf ~/.tmux.conf
```
To load the configuration do
```bash
tmux source-file ~/.tmux.conf
```
or inside tmux:
```
:source-file ~/.tmux.conf
```

### Bash 

To install Bash configurations, paste:
```bash
ln -s ~/.dotfiles/bash/bashrc ~/.bashrc
ln -s ~/.dotfiles/bash/bash_logout ~/.bash_logout
```

### Git 

To install Git configurations, paste:
```bash
ln -s ~/.dotfiles/git/gitconfig ~/.gitconfig
ln -s ~/.dotfiles/git/gitignore_global ~/.gitignore_global
```
