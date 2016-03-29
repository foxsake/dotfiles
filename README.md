This repository holds my configuration files so that I can clone them to other machines easily.

## Installation

Go to home directory and paste:

```bash
git clone https://github.com/foxsake/dotfiles ~/.dotfiles
```

### Vim

To install vim, paste:
```bash
ln -s ~/.dotfiles/vim/vim ~/.vim 
ln -s ~/.dotfiles/vim/vimrc ~/.vimrc
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
``````bash
git submodule foreach git pull origin master
```

### Tmux
To install tmux, paste:
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

To install Bash, paste:
```bash
ln -s ~/.dotfiles/bash/bashrc ~/.bashrc
ln -s ~/.dotfiles/vim/bash_logout ~/.bash_logout
```
