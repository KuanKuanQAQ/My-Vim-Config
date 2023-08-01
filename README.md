# Vim Config

## 0. 安装

1. 进入 Home 目录 `cd ~`
2. 执行 `git clone https://github.com/poettian/vim.git .vim`
3. 复制 vim 配置文件 `cp .vim/.vimrc.example .vimrc`
4. 打开 vim，执行命令 `:PlugInstall`

## 1. 关于插件

vim 传统的插件组织形式是将插件分拆为几个部分分别放到不同的目录，如下：

`~/.vim/colors/`

Vim将会查找该目录下的配色文件并执行它。这个文件应该包括生成你的配色方案所需的一切Vim script命令。

`~/.vim/plugin/`

该目录下的文件将在每次Vim启动的时候执行。这里的文件包括那些无论何时，在启动Vim之后你就想加载的代码。

`~/.vim/autoload/`

autoload是一种延迟插件代码到需要时才加载的方法。举个例子：当在 .vimrc 中使用了一个未定义的函数，vim会自动去 autoload 目录下的文件中查找是否有此函数的定义。

## 2. 插件管理器

显然，自己写插件是一件费时费力的事，如果有人帮你干了，又何必再去造轮子。

我使用的管理器是 [vim-plug](https://github.com/junegunn/vim-plug)，安装很简单，只要把 `plug.vim` 放入 ~/.vim/autoload 目录下即可。

vim-plug 的配置可以参考其文档。

## 3. nerdtree
