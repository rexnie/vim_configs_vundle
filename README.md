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
  
