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
ln -sf ~/dotfiles/tmux.conf ~/.tmux.conf
```

Since 01.2016. themes for vim-airline status bar are maintained separetely.
To install those themes, run the following:

```bash
git clone https://github.com/vim-airline/vim-airline-themes.git
cd vim-airline-themes/autoload/airline/themes
cp * ~/.vim/pack/my-plugins/start/vim-airline/autoload/airline/themes/
cd ../../../../.. && rm -rf vim-airline-themes
```
