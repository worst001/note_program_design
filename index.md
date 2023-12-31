<!-- PROJECT SHIELDS -->

[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]
[![Stargazers][stars-shield]][stars-url]
<!-- [![LinkedIn][linkedin-shield]][linkedin-url] -->

<!-- PROJECT LOGO -->

# 编辑与模式

## 什么是程序编辑

程序编辑指的是使用程序编辑器（文本编辑器或集成开发环境IDE）编写和修改源代码的过程。程序编辑器是软件开发人员用来创建、编辑、管理和查看源代码的工具。它们通常提供多种功能来帮助程序员高效编码，如语法高亮、代码自动完成、错误检测等。

### 常见的程序编辑器和编辑工具
+ Markdown - 程序以及文档编辑强力语言工具
+ Latex - PDF文档、数学公式展示的强力工具，以及事实上的标准
+ Matlab - 数学公式与算法编辑的工具
+ Tmux - Linux 终端会话与设计的工具，与Shell、Vim结合能发挥强大的功能
+ Vim、Emacs - 轻量级且功能强大的源代码编辑器，其他常用的工具还有 Visual Studio Code, Sublime Text, Atom, Eclipse, IntelliJ IDEA, PyCharm, Xcode等

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

--------------------

## Markdown

### 参考文档

[基本语法与用法](Markdown/README/README.md)

[表情emoji](Markdown/README/emoji.md)

[官方教程](https://markdown.com.cn/basic-syntax/)

[如何在Github上写出漂亮的README](Markdown/如何在github上写出漂亮的readme.md)

[mkdocs](https://www.mkdocs.org/getting-started/)


### 基本介绍

Markdown是一种轻量级的标记语言，设计用于简化文本的编写和格式化。它使用简单的标记符号来表示文本的结构和样式，具有易读、易写的特点。

### 主要特点和常用语法

#### 简洁易读
Markdown使用纯文本编写，没有复杂的标记和语法，易于阅读和编辑。

#### 标题
使用 # 符号表示标题，数量表示标题级别（例如 # 标题1 表示一级标题）。

#### 段落和换行
使用空行来分隔段落，换行可以通过在行尾添加两个空格或使用 <br> 标签实现。

#### 强调和斜体
使用 * 或 _ 符号包围文本来表示强调或斜体效果。

#### 链接
使用 `[链接文本](链接地址)` 的格式创建链接，也可以使用 <链接地址> 来创建自动链接。

#### 图片
使用 `![替代文本](图片地址)` 的格式插入图片。

#### 列表
使用 - 或 * 符号开头表示无序列表，使用数字加.表示有序列表。

#### 引用
使用 > 符号表示引用内容。

#### 代码块
使用反引号 \` 包围单行代码，使用三个反引号 \`\`\` 包围多行代码块。

#### 分割线
使用三个或更多的 -、* 或 _ 符号创建分割线。

### 总结
Markdown可以用于各种场景，如撰写文档、编写博客、发布文章、编写README文件等。许多平台和编辑器都支持Markdown格式，例如GitHub、Stack Overflow、VS Code等。


--------------------------

## Latex

### 参考文档

[Latex 自用脑图](https://www.yuque.com/hanwenhao-bs03y/tncnv7/iy0aay0hgghfhqgn?singleDoc# 《Latex》)

[Latex 中文手册](https://albertyzp.github.io/2019/10/15/LaTex%E5%9F%BA%E7%A1%80%E6%89%8B%E5%86%8C/#%E4%B8%80-latex%E5%9F%BA%E6%9C%AC%E6%A6%82%E5%BF%B5)


### 基本介绍

LaTeX是一种专业的排版系统，用于创建高质量的科技文档、学术论文、书籍、演示文稿等。它基于TeX排版引擎，提供了丰富的功能和灵活的控制选项，使得用户可以通过代码编写来精确控制文档的样式和格式。

### 主要特点和常用语法

#### 强大的数学公式支持
LaTeX在处理数学公式和符号方面非常出色，具有广泛的数学符号库和专业的排版规则。

#### 结构化文档
LaTeX鼓励使用结构化的方式来编写文档，如章节、段落、列表等，并可自动生成目录、参考文献等。

#### 专业的排版效果
LaTeX提供了丰富的排版命令和环境，允许用户对字体、段落、标题、页眉页脚等进行细致的控制，以实现专业的排版效果。

#### 参考文献管理
LaTeX提供了强大的参考文献管理系统（如BibTeX），使得引用和生成参考文献列表变得简单和一致。

#### 图片和表格插入
LaTeX支持插入高质量的图片和表格，并提供了灵活的布局和排列选项。

#### 自定义样式
LaTeX允许用户根据自己的需求和喜好定义自己的样式文件，以适应不同的出版规范和风格要求。

#### 跨平台和开源
LaTeX是跨平台的，可在各种操作系统上运行，并且是开源的，拥有庞大的用户社区和资源支持。

### 总结
LaTeX使用基于文本的命令语法，通过编写LaTeX代码来生成最终的文档。用户可以使用任何文本编辑器编写LaTeX代码，并使用LaTeX编译器（如pdfTeX、XeTeX、LuaTeX等）将代码编译成PDF或其他格式的文档。

LaTeX在学术界、科研领域和出版界广泛使用，因为它能够产生高质量、专业的文档，并提供了对复杂数学公式和结构化文档的优秀支持。尽管LaTeX需要一些学习曲线，但一旦掌握，它可以成为一个强大而灵活的工具来创建精美的文档。


--------------------------

## Matlab

### 参考文档

[Matlab 官方手册](https://ww2.mathworks.cn/help/matlab/)

### 基本介绍

MATLAB是一种强大的数值计算和科学编程环境，常用于工程、科学和数学领域的数据分析、算法开发和可视化。它提供了丰富的工具箱和函数库，使得用户能够进行各种复杂的数值计算、数据处理和模拟实验。

### 主要特点和功能

#### 数值计算
MATLAB具有高效的数值计算引擎，支持矩阵和向量操作、线性代数、统计分析、傅里叶变换等数学运算。

#### 数据可视化
MATLAB提供了强大的绘图和可视化功能，可以创建二维和三维图形、动画、图像处理和交互式界面，以便更好地理解和展示数据。

#### 算法开发
MATLAB是一个优秀的算法开发平台，用户可以通过编写脚本和函数来实现自定义的数值算法、模型仿真和优化问题求解。

#### 数据处理和分析
MATLAB提供了丰富的数据处理和分析工具，如数据预处理、滤波、插值、拟合曲线、分类、聚类等，方便用户对复杂数据进行处理和分析。

#### 应用开发
MATLAB支持应用程序开发，用户可以创建自己的GUI界面、构建完整的应用程序，并与其他编程语言（如C/C++、Python等）进行集成。

#### 工具箱和函数库
MATLAB拥有广泛的工具箱和函数库，包括信号处理、图像处理、控制系统、机器学习、计算生物学、通信等领域的工具，方便用户在特定领域中进行专业的数据分析和建模。

### 总结
MATLAB使用MATLAB语言进行编程，语法简洁而灵活。用户可以通过命令窗口进行交互式的操作，也可以编写脚本文件（以.m为扩展名）进行批量运行和自动化处理。

MATLAB在科学研究、工程开发、教育培训等领域得到广泛应用。它的易用性、强大的数值计算能力和丰富的功能使其成为了科学计算和数据分析的首选工具之一。


--------------------------

## Tmux

### 参考文档

[Tmux](https://louiszhai.github.io/2017/09/30/tmux/)

### 基本介绍

Tmux（Terminal Multiplexer）是一个在终端窗口中运行多个终端会话的工具。它允许用户在单个终端窗口中同时运行和管理多个虚拟终端，并提供了分离和重连会话的功能。

### 主要特点和功能

#### 多窗格布局
Tmux支持将终端窗口划分为多个窗格，每个窗格可以显示不同的终端会话或命令行界面。

#### 会话管理
Tmux允许用户创建和管理多个独立的会话。用户可以在会话之间自由切换，并在后台运行会话以便在需要时重新连接。

#### 分离和重连
Tmux的一个重要特性是可以在断开连接后保持会话的状态。这意味着即使关闭了终端窗口或网络连接中断，用户也可以重新连接到之前的会话并恢复工作环境。

#### 窗口和标签
Tmux允许用户在一个会话中创建多个窗口，并为每个窗口添加标签。这样可以方便地组织和切换不同的任务或项目。

#### 自定义配置
Tmux提供了丰富的配置选项，允许用户根据自己的喜好和需求来自定义键绑定、外观和行为。

### 总结
Tmux在命令行界面下使用，并提供了一组丰富的命令和快捷键来管理终端会话和窗口布局。通过使用Tmux，用户可以更高效地利用终端窗口，同时运行和管理多个任务或会话，并实现工作环境的分离和重连。

Tmux是一个非常有用和强大的工具，特别适合那些需要同时处理多个终端会话和任务的开发人员、系统管理员和远程连接用户。


--------------------------

## Vim

### 参考文档

#### 自用配置

[Vim 自用笔记](Vim/Vim.md)

[Vim 手册](Vim/user_manual-2.4.0.pdf)

[自用 Vim 配置备份](https://github.com/worst001/nvim_0)

#### 配套工具

[NeoVim](https://github.com/neovim/neovim)

[CocNvim](https://github.com/neoclide/coc.nvim)

[Packer与Telescope](https://github.com/nvim-telescope/telescope.nvim)

[FZF](https://github.com/junegunn/fzf)

[Joshuto](https://github.com/kamiyaa/joshuto)


### 基本介绍

Vim（Vi IMproved）是一款功能强大的文本编辑器，被广泛用于命令行环境和开发工作中。它是Vi编辑器的增强版本，提供了更多的功能和灵活性。

### 主要特点和功能

#### 模式
Vim具有多种模式，包括普通模式、插入模式、可视模式和命令行模式。在不同的模式下，用户可以执行各种编辑操作和命令。

#### 快速移动和编辑
Vim提供了丰富的快捷键和命令来高效地进行光标移动、文本选择、复制粘贴、删除、替换等编辑操作。

#### 可定制性
Vim支持丰富的配置选项和插件系统，允许用户根据自己的需求和喜好进行个性化设置和扩展功能。

#### 强大的搜索和替换
Vim提供了强大的搜索和替换功能，支持正则表达式和全局替换，可以快速查找和修改文本内容。

#### 分割窗口
Vim允许用户将编辑区域划分为多个水平或垂直的分割窗口，方便同时编辑多个文件或查看不同部分的代码。

#### 多语言支持
Vim支持多种编程语言，提供了语法高亮、自动缩进、代码折叠等功能，使得编码更加方便和可读。

#### 远程编辑
Vim可以通过SSH或其他远程连接方式进行远程编辑，方便在服务器上编辑文件。

### 总结
Vim是一个高度可定制且极具效率的文本编辑器，它的学习曲线可能较陡峭，但一旦掌握，用户可以以非常快速和高效的方式进行文本编辑和开发工作。它被广泛用于Linux和Unix系统中，并支持Windows和Mac OS X等操作系统。


--------------------------

## Emacs

### 参考文档

[SpaceEmacs](https://www.spacemacs.org/)

[Lisp](https://oneforalone.github.io/cl-cookbook-cn/#/)

[MELPA 中心](https://melpa.org/#/)

### 基本介绍

Emacs是一款功能强大的可扩展文本编辑器，广泛用于编程、文档撰写和其他文本处理任务。它具有高度可定制性和丰富的功能，被认为是一种操作系统级别的编辑环境。

### 主要特点和功能

#### 文本编辑
Emacs提供了全面的文本编辑功能，包括查找替换、剪切复制粘贴、撤销重做、缩进自动补全等。

#### 扩展性
Emacs允许用户通过Lisp编程语言来扩展和自定义其功能。用户可以编写脚本和插件来添加新的命令、编辑模式、函数和工具。

#### 多窗口和分割窗格
Emacs支持在一个编辑器实例中同时打开多个文件，并提供了灵活的窗口管理功能，包括水平和垂直的窗格分割、切换焦点等。

#### 代码编辑和调试
Emacs针对不同编程语言提供了丰富的代码编辑和开发环境，包括语法高亮、自动补全、代码折叠、编译和调试等功能。

#### 文件管理和版本控制
Emacs集成了文件和目录管理功能，可以浏览和操作文件系统。此外，它也支持常见的版本控制系统，如Git和SVN。

#### 文档查阅和阅读
Emacs可以打开各种文档格式，包括纯文本、PDF、HTML等。它还提供了浏览和搜索文档的功能。

#### 电子邮件和日历
Emacs内置了电子邮件客户端（Gnus）和日历管理工具，方便用户处理邮件和日程安排。

### 总结
Emacs是一个非常灵活和可定制的编辑器，但也有一定的学习曲线。它提供了丰富的命令和快捷键，以及强大的扩展能力，适用于那些对编辑器进行高度定制并希望在一个环境中处理多种任务的用户。


--------------------------

## 设计模式

### 参考文档

[为了人类的设计](设计模式/design-patterns-for-humans-cn/README.md)

[理论与详解](https://refactoringguru.cn/design-patterns/catalog)

[各语言模板总览](https://github.com/DovAmir/awesome-design-patterns)


### 基本介绍

设计模式（Design Patterns）是软件设计中常见问题的典型解决方案。它们是在多年软件开发实践中总结出来的，用以解决特定上下文中重复出现的设计问题。设计模式可以提高代码的可重用性、可读性和可维护性，并且可以改进系统的设计质量。

#### 设计模式通常被分成三类

+ 创建型（Creational）
+ 结构型（Structural）
+ 行为型（Behavioral）

#### 创建型模式

创建型模式关注对象创建的不同方式。目的是创建对象时，增加程序的灵活性和复用性。

+ 单例（Singleton）：确保一个类只有一个实例，并提供一个全局访问点。
+ 简单工厂（Simple Factory）：一个工厂类根据传入的参数决定创建出哪一种产品类的实例，但不属于GOF提出的23种设计模式。
+ 工厂方法（Factory Method）：定义了一个创建对象的接口，让子类决定实例化哪一个类。
+ 抽象工厂（Abstract Factory）：允许创建一系列相关或互相依赖的对象，而不需要指定具体的类。
+ 建造者（Builder）：将一个复杂对象的构建与它的表示分离，同样的构建过程可以创建不同的表示。
+ 原型（Prototype）：通过复制现有的实例来创建新的实例，而不是新建实例。

#### 结构型模式
结构型模式涉及到如何组合类和对象以获得更大的结构。

+ 适配器（Adapter）：允许不兼容的接口可以一起工作。
+ 桥接（Bridge）：将抽象部分与实现部分分离，使它们可以独立变化。
+ 组合（Composite）：将对象组合成树形结构以表示部分-整体层次结构，使用户对单个对象和组合对象的使用具有一致性。
+ 装饰（Decorator）：动态地给一个对象添加一些额外的职责，就增加功能来说，它提供了比继承更有弹性的替代方案。
+ 外观（Facade）：提供一个统一的接口以访问子系统中的一群接口，从而使子系统更容易被使用。
+ 享元（Flyweight）：运用共享技术有效地支持大量细粒度的对象。
+ 代理（Proxy）：提供一个替代品或占位符来代表一个重量级对象，从而控制对它的访问。

#### 行为型模式
行为型模式专注于对象间的通信。

+ 责任链（Chain of Responsibility）：使多个对象都有机会处理请求，从而避免请求的发送者和接收者之间的耦合关系。
+ 命令（Command）：将一个请求封装为一个对象，从而使你可用不同的请求对客户进行参数化。
+ 解释器（Interpreter）：给定一个语言，定义它的文法的一种表示，并定义一个解释器。
+ 迭代器（Iterator）：提供一种方法顺序访问一个集合对象中各个元素，而不暴露其内部的表示。
+ 中介者（Mediator）：用一个中介对象来封装一系列的对象交云。
+ 备忘录（Memento）：捕捉一个对象的内部状态，以便在将来的某个时刻可以恢复它的状态。
+ 观察者（Observer）：当一个对象变化时，会自动通知它的依赖对象。
+ 状态（State）：允许一个对象在其内部状态改变时改变它的行为。
+ 策略（Strategy）：定义一系列的算法，把它们一个个封装起来，并且使它们可以互换。
+ 模板方法（Template Method）：定义一个操作中算法的骨架，而将一些步骤延迟到子类中。
+ 访问者（Visitor）：表示一个作用于某对象结构中的各元素的操作。它可以在不改变各元素的类的前提下定义作用于这些元素的新操作。


<!-- links -->
[your-project-path]:shaojintian/Best_README_template
[contributors-shield]: https://img.shields.io/github/contributors/worst001/note_program_design.svg?style=flat-square
[contributors-url]: https://github.com/worst001/note_program_design/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/worst001/note_program_design.svg?style=flat-square
[forks-url]: https://github.com/worst001/note_program_design/network/members
[stars-shield]: https://img.shields.io/github/stars/worst001/note_program_design.svg?style=social
[stars-url]: https://github.com/worst001/note_program_design/stargazers
[issues-shield]: https://img.shields.io/github/issues/worst001/note_program_design.svg?style=flat-square
[issues-url]: https://img.shields.io/github/issues/worst001/note_program_design.svg
[license-shield]: https://img.shields.io/github/license/worst001/note_program_design.svg?style=flat-square
[license-url]: https://github.com/worst001/note_program_design/blob/main/LICENSE.txt
