# 说明
使用stow管理dotfile
stow是一个管理symble link的工具, 能够以目录为单位, 把给定目录下的文件软链接到目标目录下

stow的安装: `brew install stow`

比如: `stow -d $HOME/dotfiles -t $HOME git` 把 \$HOME/dotfiles/git 目录下的所有文件都软链接到$HOME目录下. 如果-d没有指定, 默认是当前目录. 如果-t没有指定, 默认是当前目录的上层目录. 所以实际上可以在本dotfile目录下: `stow git`, `stow shell`

# 目录介绍

* **git**: 这是全局git配置, 包括.gitconfig与.gitignore_global
* **shell**: 这是shell的配置文件, 包括.bashrc与.zshrc