<a name="readme-top"></a>
<!-- PROJECT SHIELDS -->

[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]
<!-- [![LinkedIn][linkedin-shield]][linkedin-url] -->

<!-- PROJECT LOGO -->

<!-- 项目LOGO -->
<br />
<div align="center">
  <!-- <a href="http://mkdocs.grft.top"> -->
  <!--   <img src="https://xiyou-oss.oss-cn-shanghai.aliyuncs.com/mkdocs/logo.png" alt="Logo" width="480" height="270"> -->
  <!-- </a> -->

  <h3 align="center">编辑与模式</h3>

  <p align="center">
    <br />
    <a href="http://mkdocs.grft.top/编辑与模式/"><strong>探索文档 »</strong></a>
    <br />
  </p>
</div>

<!-- 目录 -->
<details>
  <summary>目录</summary>
  <ol>
    <li><a href="#关于项目">关于项目</a></li>
    <li><a href="#什么是程序编辑">什么是程序编辑</a></li>
    <li><a href="#什么是设计模式">什么是设计模式</a></li>
    <li><a href="#技术目录">技术目录</a></li>
    <li><a href="#贡献">贡献</a></li>
    <li><a href="#许可证">许可证</a></li>
    <li><a href="#联系方式">联系方式</a></li>
    <li><a href="#鸣谢">鸣谢</a></li>
  </ol>
</details>


## 关于项目

整理了程序设计中需要用到的编辑工具资料、笔记与手册

整理了23种常用设计模式以及其不同语言下的模板

公网资料、笔记地址请访问这里 

- 文档地址: [http://mkdocs.grft.top/编辑与模式/](http://mkdocs.grft.top/编辑与模式/)

其他相关技术可以访问我的博客，主页地址请访问这里

- 访问入口：[http://mkdocs.grft.top](http://mkdocs.grft.top)

<p align="right">(<a href="#readme-top">回到顶部</a>)</p>


## 什么是程序编辑

程序编辑指的是使用程序编辑器（文本编辑器或集成开发环境IDE）编写和修改源代码的过程。程序编辑器是软件开发人员用来创建、编辑、管理和查看源代码的工具。它们通常提供多种功能来帮助程序员高效编码，如语法高亮、代码自动完成、错误检测等。

### 常见的程序编辑器和编辑工具
+ Markdown - 程序以及文档编辑强力语言工具
+ Latex - PDF文档、数学公式展示的强力工具，以及事实上的标准
+ Matlab - 数学公式与算法编辑的工具
+ Tmux - Linux 终端会话与设计的工具，与Shell、Vim结合能发挥强大的功能
+ Vim、Emacs - 轻量级且功能强大的源代码编辑器，其他常用的工具还有 Visual Studio Code, Sublime Text, Atom, Eclipse, IntelliJ IDEA, PyCharm, Xcode等

<p align="right">(<a href="#readme-top">回到顶部</a>)</p>


## 什么是设计模式

设计模式是软件工程中的一套被反复使用、大家公认的、最有效的解决特定问题的方案。设计模式以标准化的方式解决软件设计中经常遇到的问题，从而提高代码的复用性、可维护性和通信的清晰度。

设计模式通常按照面向对象设计原则编写，像是单一职责原则、开闭原则、里氏替换原则等。学习并正确应用设计模式可以帮助开发者创建既灵活又可扩展的软件系统。

### 设计模式主要分为三种类型

#### 创建型模式
涉及对象实例化，用于帮助创建对象实例。例如：单例（Singleton）、工厂方法（Factory Method）、抽象工厂（Abstract Factory）、建造者（Builder）和原型（Prototype）模式。

#### 结构型模式
涉及到将类或对象组织成更大的结构。例如：适配器（Adapter）、装饰器（Decorator）、代理（Proxy）、外观（Facade）、桥接（Bridge）、组合（Composite）和享元（Flyweight）模式。

#### 行为型模式
特别关注对象之间的通信。例如：策略（Strategy）、观察者（Observer）、命令（Command）、备忘录（Memento）、迭代器（Iterator）、中介者（Mediator）、状态（State）和访问者（Visitor）模式。

<p align="right">(<a href="#readme-top">回到顶部</a>)</p>

## 技术目录

[目录与大纲](index.md)

### Markdown

+ [基本语法与用法](Markdown/README/README.md)
+ [表情emoji](Markdown/README/emoji.md)
+ [官方教程](https://markdown.com.cn/basic-syntax/)
+ [如何在Github上写出漂亮的README](Markdown/如何在github上写出漂亮的readme.md)
+ [mkdocs](https://www.mkdocs.org/getting-started/)

### Latex

+ [Latex 自用脑图](https://www.yuque.com/hanwenhao-bs03y/tncnv7/iy0aay0hgghfhqgn?singleDoc#%20《Latex》)
+ [Latex 中文手册](https://albertyzp.github.io/2019/10/15/LaTex%E5%9F%BA%E7%A1%80%E6%89%8B%E5%86%8C/#%E4%B8%80-latex%E5%9F%BA%E6%9C%AC%E6%A6%82%E5%BF%B5)


### Matlab

+ [Matlab 官方手册](https://ww2.mathworks.cn/help/matlab/)


### Tmux

+ [Tmux](https://louiszhai.github.io/2017/09/30/tmux/)


### Vim

#### 自用配置

+ [Vim 自用笔记](Vim/Vim.md)
+ [Vim 手册](Vim/user_manual-2.4.0.pdf)
+ [自用 Vim 配置备份](https://github.com/worst001/nvim_0)

#### 配套工具

+ [NeoVim](https://github.com/neovim/neovim)
+ [CocNvim](https://github.com/neoclide/coc.nvim)
+ [Packer与Telescope](https://github.com/nvim-telescope/telescope.nvim)
+ [FZF](https://github.com/junegunn/fzf)
+ [Joshuto](https://github.com/kamiyaa/joshuto)


### Emacs

+ [SpaceEmacs](https://www.spacemacs.org/)
+ [Lisp](https://oneforalone.github.io/cl-cookbook-cn/#/)
+ [MELPA 中心](https://melpa.org/#/)


### 设计模式

+ [为了人类的设计](设计模式/design-patterns-for-humans-cn/README.md)
+ [理论与详解](https://refactoringguru.cn/design-patterns/catalog)
+ [各语言模板总览](https://github.com/DovAmir/awesome-design-patterns)


<p align="right">(<a href="#readme-top">回到顶部</a>)</p>

<!-- 贡献 -->

## 贡献

贡献是使开源社区成为一个如此令人惊叹的地方，以学习、激励和创造。您所做的任何贡献都将非常感谢。

如果您对使这个项目变得更好有建议，请 fork 该仓库并创建 pull request。您也可以打开一个带有“enhancement”标签的问题。不要忘记给这个项目点个星！再次感谢！

<p align="right">(<a href="#readme-top">返回顶部</a>)</p>


<!-- 许可证 -->
## 许可证

根据 MIT 许可证进行分发。更多信息请参见 [LICENSE.txt](LICENSE)。

<p align="right">(<a href="#readme-top">返回顶部</a>)</p>

<!-- 联系方式 -->
## 联系方式

关注我: [小昊子](https://github.com/worst001)

博客地址: [http://mkdocs.grft.top](http://mkdocs.grft.top)

项目链接: [https://github.com/worst001/mkdocs_program_design](https://github.com/worst001/mkdocs_program_design)

<p align="right">(<a href="#readme-top">返回顶部</a>)</p>

## 鸣谢

因为仓库与文档的数量比较大，有些借鉴资料忘了在`参考文档`部分提及原作者与原仓库，若有疏漏请告诉，我及时补上。

所有引用的原资料都确认是开源认证，若有侵权请告知。

[https://github.com/younghz/Markdown](https://github.com/younghz/Markdown)

[https://www.mkdocs.org/getting-started/](https://www.mkdocs.org/getting-started/)

[https://github.com/theniceboy/nvim](https://github.com/theniceboy/nvim)

[https://github.com/doomemacs/doomemacs](https://github.com/doomemacs/doomemacs)

[https://github.com/kamranahmedse/design-patterns-for-humans](https://github.com/kamranahmedse/design-patterns-for-humans)

[https://github.com/JakubVojvoda/design-patterns-cpp](https://github.com/JakubVojvoda/design-patterns-cpp)

[https://github.com/iluwatar/java-design-patterns](https://github.com/iluwatar/java-design-patterns)

[https://github.com/nikolovivan/scala-design-patterns](https://github.com/nikolovivan/scala-design-patterns)

[https://github.com/DesignPatternsPHP/DesignPatternsPHP](https://github.com/DesignPatternsPHP/DesignPatternsPHP)

[https://github.com/faif/python-patterns](https://github.com/faif/python-patterns)

[https://github.com/senghoo/golang-design-pattern](https://github.com/senghoo/golang-design-pattern)

[https://github.com/QianMo/Unity-Design-Pattern](https://github.com/QianMo/Unity-Design-Pattern)

[https://github.com/fbeline/design-patterns-JS](https://github.com/fbeline/design-patterns-JS)

[https://github.com/woshihuo12/LuaDesignPattern](https://github.com/woshihuo12/LuaDesignPattern)

[https://openai.com/chatgpt](https://openai.com/chatgpt)


<!-- links -->
[your-project-path]:shaojintian/Best_README_template
[contributors-shield]: https://img.shields.io/github/contributors/worst001/mkdocs_program_design.svg?style=flat-square
[contributors-url]: https://github.com/worst001/mkdocs_program_design/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/worst001/mkdocs_program_design.svg?style=flat-square
[forks-url]: https://github.com/worst001/mkdocs_program_design/network/members
[stars-shield]: https://img.shields.io/github/stars/worst001/mkdocs_program_design.svg?style=flat-square
[stars-url]: https://github.com/worst001/mkdocs_program_design/stargazers
[issues-shield]: https://img.shields.io/github/issues/worst001/mkdocs_program_design.svg?style=flat-square
[issues-url]: https://img.shields.io/github/issues/worst001/mkdocs_program_design.svg
[license-shield]: https://img.shields.io/github/license/worst001/mkdocs_program_design.svg?style=flat-square
[license-url]: https://github.com/worst001/mkdocs_program_design/blob/main/LICENSE.txt
<!-- [linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=flat-square&logo=linkedin&colorB=555 -->
<!-- [linkedin-url]: https://linkedin.com/in/shaojintian -->
