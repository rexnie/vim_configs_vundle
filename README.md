# vim_configs_vundle

用vundle来管理繁多的vim插件，非常方便。

参考: https://github.com/Li-Wenhui/VimLeo

# 如何使用该库

1. clone 该库
  ```
  cd ~/.vim/
  rm ./* -rf
  git clone https://github.com/rexnie/vim_configs_vundle.git .
  cp ~/.vim/_vimrc ~/.vimrc
  ```
2. 安装 Vundle 及其他 plugin
  ```
  git clone https://github.com/VundleVim/Vundle.vim.git ~/.vim/bundle/Vundle.vim
  vim +PluginInstall +qall
  ```
  
# 源码安装编辑器 vim
1. 在 ubuntu 20.04 源码安装 vim
  ```
sudo apt-get install python-dev python3-dev ruby-dev liblua5.2-dev liblua5.3-dev libx11-dev libgtk-3-dev libgtk2.0-dev ncurses-dev lua5.2
git clone https://github.com/vim/vim.git
cd vim/
git checkout v8.0.0000
./configure --with-features=huge --enable-pythoninterp --enable-rubyinterp --enable-luainterp --enable-perlinterp --with-python-config-dir=/usr/lib/python2.7/config/ --enable-gui=gtk2 --enable-cscope --prefix=/usr
make
sudo make install
  ```
  需要checkout v8.0是因为 8.2的 vim 还不能很好的支持 neocomplete。
