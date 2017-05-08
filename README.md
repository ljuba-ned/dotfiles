# Usage

Clone this repo and make appropriate symbolic links

```bash
cd ~
git clone https://github.com/ljuba-ned/dotfiles.git dotfiles
cd dotfiles
# vim plugins are mainly submodules, initialize
git submodule init
git submodule update
# vim symlinks, if you already have .vim and .vimrc in your
# home directory, rename them
ln -sf ~/dotfiles/vim/vimrc ~/.vimrc
ln -sf ~/dotfiles/vim ~/.vim
# symlink for tmux configuration
ln -sf ~/dotfiles/.tmux.conf ~/.tmux.conf
```

