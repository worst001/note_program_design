# Vim 自用笔记

## 简介

### 什么是 Vim

> Vim 本质上就是一款文本编辑器，它在Vi的基础上改进和增加了很多特性。
> Vim本身拥有自己的脚本语言Vimscript
> Vim是高度可定制的文本编辑器，可以使用Vimscript达到高度可定制。
> Vim是开源的自由软件，不收费。
> Vim属于Unix生态

### Vim 能做什么

> 当记事本使用
> 代码编写并支持所有语言
> 通过shell与其他语言完成各种各样丰富的工作
(Emacs可以煮咖啡 Vim也能)

## 基础语法

### 设置

#### 配置文件
1. vimrc
> 某个Unix用户的家目录下的入口配置文件
> 该用户登录后使用该.vimrc的配置文件
> 严格意义上.vim结尾的文件才是Vimscript
2. source
> source命令可以立刻加载某个vim脚本

#### 系统设置
1. 系统字段
> filetype  文件类型识别
> set       设置vim内置的功能
> syntax    语法高亮

2. 示例
```vim
:filetype on                                    " 文件类型识别开启
:filetype indent on                             " 开启缩进
:filetype plugin on                             " 开启插件
:set fencs=utf-8,chinese fenc=utf-8 enc=utf-8   " 编码设置成UTF-8
:syntax on                                      " 代码高亮

augroup basic
  autocmd!
  autocmd BufReadPost * :let &t_ut=''
  autocmd BufReadPost * :set expandtab          " tab转化成空格
  autocmd BufReadPost * :set smarttab           " 智能判断缩进的空格数
  autocmd BufReadPost * :set autoindent         " 自动缩进
  autocmd BufReadPost * :set number             " 开启行号
  autocmd BufReadPost * :set relativenumber     " 开启相对行号
  autocmd BufReadPost * if line("'\"") > 1 && line("'\"") <= line("$") | exe "normal! g'\"" | endif " 记录上一次文件抒写点
augroup END

set mouse=a                   " 开启鼠标控制
set cursorline                " 光标所处行高亮
" set cursorcolumn            " 光标所处列高亮
set guicursor=i:ver50-iCursor-blinkon1,n-c-v:block-ncvCursor-blinkoff1  " 光标normal模式时静止, insert模式闪烁
set list                      " 显示特殊字符
set nowrap                    " 越界的行不换行
set foldmethod=indent         " 按照缩进的方式进行折叠
set foldlevel=99              " 折叠等级设置为99
set foldenable                " 开启折叠
set hlsearch                  " 高亮查询的结果
set incsearch                 " 在输入搜索字符时就高亮
set ignorecase                " 忽略大小写
set smartcase                 " 如果包含大写就区分大小写
set scrolloff=5               " 滚动激活的边距
set listchars=tab:▸\ ,trail:▫ " 特殊字符展示的效果
set laststatus=2              " 开启状态行

```

### 模式

#### 几种模式
1. 普通模式 normal
可以认为是浏览模式 光标可以自由的移动 这个模式下有大量的*操作符*可以使用

2. 插入模式 insert
手动输入字符 光标随着输入的字符后移

3. 可视模式 visual
光标移动时会框选区域 对框选某一个区域也可做处理

4. 替换模式 replace
每次输入都会覆盖之前的字符(不常用)

#### 模式映射

```vim
:let mapleader="\<Space>"       " 操作前缀

" normal 模式
:nnoremap <leader>sx  :source %<cr>
:nnoremap <silent>yp  :let @+ = expand('%:p:h')<cr>

" insert 模式
:inoremap jk          <esc>

" visual 模式
:vnoremap K           9k

" visual 和 normal都执行
":noremap  K           9k
:noremap  J           9j
:noremap  L           12l
:noremap  H           12h
:noremap  S           :w<cr>
:noremap  --          :join<cr>
```

### 操作符(重点)

#### Vim 键位图
![键位图](./vim操作键位图.png)

#### 操作符映射
```vim
:onoremap i(          :<c-u>normal!   f(vi(<cr>
:onoremap i[          :<c-u>normal!   f[vi[<cr>
:onoremap i{          :<c-u>normal!   f{vi{<cr>

"aaaaa(bbb-ccccc)
"aaaaa[bbb-ccccc]
"aaaaa{bbb-ccccc}
```

### 自动命令

#### 定义
打开vim时自动执行某些命令

#### 示例
```vim
augroup filetype_vim
  autocmd!
  autocmd FileType vim  :set tabstop=2
  autocmd FileType vim  :set shiftwidth=2
  autocmd FileType vim  :set softtabstop=2
augroup END
```

### 通用语法

#### 变量
```vim
:let g:hello = "world" "全局变量
:let b:hello = "world" "当前缓冲区(当前文件)
function! SomeFunc(hello)
    " 局部变量
    echo a:hello
endfunction
```

#### 流程
```vim
" 条件语句
:if 10 > 1
:    echom "foo"
:endif

" 循环语句
:let c = 0

:for i in [1, 2, 3, 4]
:  let c += i
:endfor

:echom c
```

#### 函数
```vim
nnoremap <silent> <leader>jd   :call <SID>SomeFunc("Hello")<cr>
function! s:SomeFunc(hello)
    echo a:hello
endfunction
```

### 自定义扩展
> 熟悉vim基本语法之后就可以自己定制插件
> 插件封装在 .vim/plugin 路径下
> history 插件展示

## 经典功能

### 列向选择
<c-v> 可以进入列向选择
当某一行内容发生了变化剩余的所有行都有同样变化

### 查询与替换

#### 查询
/ 开始向下查询
? 开始向上查询
n 下一个匹配
N 上一个匹配

#### 替换
:s 部分替换
:%s 全局替换

### 宏录制
normal 模式下按 q 作为录制前缀
配合任意字母(比如a)
那么在a这个寄存器中将记录接下来的录制
```html
<a href="">aaa</a>
<a href="">bbb</a>
<a href="">ccc</a>
<a href="">ddd</a>
<a href="">eee</a>
aaa
bbb
ccc
ddd
eee
```

### 模板组件

#### vim自带模板
```vim
:iabbrev @@  hanwenhao@mail.xiyouwangluo.top
```

#### snips方案

+ 完整的代码块方案
+ 每种开发工具都有自己的代码块方案
+ 本质上是对代码文件做处理
+ 可以基于python进一步做扩展
    + http://vimcasts.org/episodes/ultisnips-python-interpolation/
+ 自用python扩展示例

```snippets
global !p
def list_params(params):
	list = params.split(',')
	link = ""
	initial_indent = snip._initial_indent
	for it in list:
		it = "\n" + initial_indent + "* @param " + it.strip() + " <+Comment+>"
		link = link + it
	return "*" + link
endglobal

snippet ff "Java Easy func" b
/**
* `!p snip.rv = t[3][0].upper()  + t[3][1:]`
* ${6:<+Description+>}
`!p snip.rv = list_params(t[4])`
*
* @return ${5:<+Return+>}
*/
${1:public} ${2:void} ${3:funcname} (${4}) {
	${7}
}
endsnippet

```



### FZF
+ 一款基于Unix的模糊查询工具
+ 用Go语言编写性能有很大的保障
+ Windows也适配
+ 底层文件、文本引擎选择
    + 传统的 find、ack 较慢
    + fd 文件查找速度最快
    + ag 巨量代码搜索非常快
    + rg 不亚于ag且对中文支持很好

## 生态

### 插件
+ idea
    + ideavim
    + 可以通过.ideavimrc 以及actionList查看idea提供的vim命令
+ eclipse
    + vrapper
    + viplugin
+ vscode
    + VimL

### 终端工具
+ tmux
    + linux上的终端管理利器
+ ranger
    + unix上的以终端形式存在的文件管理利器

### 当前的最优解决方案
+ neovim
    + 无缝支持python2、python3、nodejs、ruby、lua
    + 可以通过shell调用go、java、c++这些语言编译后的执行文件

### 自用 Vim 配置

```vim
"-------------------------------------------------------
" _   _                               _                 
"| | | | __ _ _ ____      _____ _ __ | |__   __ _  ___  
"| |_| |/ _` | '_ \ \ /\ / / _ \ '_ \| '_ \ / _` |/ _ \ 
"|  _  | (_| | | | \ V  V /  __/ | | | | | | (_| | (_) |
"|_| |_|\__,_|_| |_|\_/\_/ \___|_| |_|_| |_|\__,_|\___/ 
"                                                       
"__     ___                    
"\ \   / (_)_ __ ___  _ __ ___ 
" \ \ / /| | '_ ` _ \| '__/ __|
"  \ V / | | | | | | | | | (__ 
"   \_/  |_|_| |_| |_|_|  \___|
"                              

" SYS ENV ---------------------- {{{
" Environment {
    " Identify platform {
        silent function! OSX()
            return has('macunix')
        endfunction
        silent function! LINUX()
            return has('unix') && !has('macunix') && !has('win32unix')
        endfunction
        silent function! WINDOWS()
            return  (has('win32') || has('win64'))
        endfunction
    " }

    " Basics {
        set nocompatible        " Must be first line
        if !WINDOWS()
            set shell=/bin/zsh
        endif
    " }

    " Windows Compatible {
        " On Windows, also use '.vim' instead of 'vimfiles'; this makes synchronization
        " across (heterogeneous) systems easier.
        if WINDOWS()
          set runtimepath=$HOME/.vim,$VIM/vimfiles,$VIMRUNTIME,$VIM/vimfiles/after,$HOME/.vim/after
        endif
    " }

    " vim-autoclose不生效的Fix {
        " https://github.com/spf13/spf13-vim/issues/780
        if &term[:4] == "xterm" || &term[:5] == 'screen' || &term[:3] == 'rxvt'
            inoremap <silent> <C-[>OC <RIGHT>
        endif
    " }
" }

" System ---------------------- {{{
:filetype on
:filetype indent on
:filetype plugin on
:set fencs=utf-8,chinese fenc=utf-8 enc=utf-8
:set fileencodings=utf-8,ucs-bom,gb18030,gbk,gb2312,cp936
:set termencoding=utf-8

:syntax on
:let g:python_host_prog  = '/usr/local/bin/python2'
:let g:python3_host_prog = '/opt/homebrew/opt/python@3.10/bin/python3.10'
:let g:ruby_host_prog    = '/opt/homebrew/lib/ruby/gems/3.1.0/bin/neovim-ruby-host'



" 插件镜像地址修改
" :let g:plug_url_format   = 'https://git::@github.com.cnpmjs.org/%s.git'
" }}}

let g:vimspector_enable_mappings = 'HUMAN'
packadd! vimspector


" Basic ---------------------- {{{
augroup basic
  autocmd!
  autocmd BufReadPost * :let &t_ut=''
  autocmd BufReadPost * :set expandtab
  autocmd BufReadPost * :set smarttab
  autocmd BufReadPost * :set autoindent
  autocmd BufReadPost * :set number
  autocmd BufReadPost * :set relativenumber
  autocmd BufReadPost * if line("'\"") > 1 && line("'\"") <= line("$") | exe "normal! g'\"" | endif
augroup END
" }}}

" 插件包引入(vim-plug)
:source $HOME/.vim/init/init-packages.vim
" UI 配置(TODO: 必须跟在package后 否则ui配置不生效)
:source $HOME/.vim/init/init-ui.vim
" Lua 插件包引入(packer)
:source $HOME/.vim/init/init-packer.vim
" 插件配置
:source $HOME/.vim/init/init-better-defaults.vim
" 按键映射
:source $HOME/.vim/init/init-keybindings.vim
" 自定义辅助
:source $HOME/.vim/init/init-assist.vim

" }}}

```


### 目录结构

```
.vim
├── README.md
├── autoload
│   ├── dbext.vim.bak
│   ├── dbext_dbi.vim.bak
│   ├── plug.vim
│   └── plug.vim.old
├── coc-settings.json
├── init
│   ├── config
│   │   └── db.vim
│   ├── init-assist.vim
│   ├── init-better-defaults.vim
│   ├── init-keybindings.vim
│   ├── init-packages.vim
│   ├── init-packer.vim
│   ├── init-ui.vim
│   └── new
├── init.vim -> /Users/hanwenhao/.vim/vimrc
├── lua
│   ├── plugin-config
│   │   ├── bufferline.lua
│   │   ├── nvim-tree.lua
│   │   ├── persisted.lua
│   │   ├── telescope.lua
│   │   └── todo-comments.lua
│   └── plugins.lua
├── pack
│   └── vimspector
│       └── opt
├── package-lock.json
├── plugged
├── plugin
│   ├── terminal-open.vim
│   ├── text-highlight.vim
│   └── vimcdoc.vim
├── sessions
│   └── default.vim
├── shell
│   ├── prettier
│   ├── scalafix
│   ├── time
│   ├── uncrustify
│   ├── xml-prettier
│   └── xml2js
├── syntax
│   └── help_cn.vim
├── tree.txt
└── vimrc
```

[Vim 配置仓库地址](https://github.com/worst001/vim_0)

## 总结
+ 也不是说用vim其他开发工具就不要了，他有强大的近乎完美编辑功能。
+ 配合其他工具一起使用，可以发挥更大功效。
+ 他像"我的世界"一样可以打造自己的房子，对程序设计着来说有很大的帮助。
