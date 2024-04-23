---
title: 杂谈 —— 为什么我使用 Visual Studio Code
date: 2023-11-21 23:10:00
updated: 2024-4-14 12:10:00
categories: Share & Misc
tags: VSCode
Front-matter: False
index_img: https://pixiv.nl/82752479.jpg
banner_img: https://pixiv.nl/82752479.jpg
---

# 前言

笔者大学计算机专业大一的入门语言是C语言，老师大多都给学生推荐集成开发环境 (IDE) 来进行程序的编写，主要就是Visual C++ 2010 和 Dev C++。这些老旧的 IDE 体验一言难尽，中世纪的界面，落后的功能，还有糟糕的调试体验，学生不少也是拿来就用了，好点的还会去网上下载一个 Visual Studio，有的学生可能拿着 DEV C++ 迷迷糊糊地就开始用了。~~不能再犹豫了，一定要出重拳！~~ 笔者作为 VSCode 的忠实用户，当然要大力宣传好用的 VSCode 了！

## 文本编辑器、编译器、集成开发环境 (IDE) 的区别

在这里插一个小知识，关于文本编辑器 (俗称编辑器)、编译器、集成开发环境 (IDE) 的区别，很多新手并没有搞清楚这些概念，老师往往也没有特意强调。

### 编辑器

>**文本编辑器**是种计算机软件，主要用来编写和查看文本文件。特殊的文本编辑器支持增加自有的格式来丰富文档的表现形式。操作系统或者集成开发环境通常会带有可以查看和编辑纯文本的编辑器，可增加格式的文本编辑器通常是个人用户或者公司在制作需要格式的文件中使用。程序和其配置档常以纯文本格式储存，程序员也须用纯文本编辑器来编辑程序和配置文件。
>
>————维基百科

文本编辑器往往并不能直接用于调试、运行你写的代码，需要安装插件，进行手动配置，配合编译器才能完成编程的整套过程；高自由度，轻量化和良好的兼容性是其最鲜明的优点。

文本编辑器的例子：记事本, VS Code, VIM, Notepad++

### 编译器

>编译器（compiler）是一种计算机程序，它会将某种编程语言写成的源代码（原始语言）转换成另一种编程语言（目标语言）。
>
>它主要的目的是将便于人编写、阅读、维护的高级计算机语言所写作的源代码程序，翻译为计算机能解读、运行的低阶机器语言的程序，也就是可执行文件。编译器将原始程序（source program）作为输入，翻译产生使用目标语言（target language）的等价程序。源代码一般为高级语言（High-level language），如Pascal、C、C++、C# 、Java等，而目标语言则是汇编语言或目标机器的目标代码（Object code），有时也称作机器代码（Machine code）。
>
>一个现代编译器的主要工作流程如下：
>
>源代码（source code）→ 预处理器（preprocessor）→ 编译器（compiler）→ 汇编程序（assembler）→ 目标代码（object code）→ 链接器（linker）→ 可执行文件（executables），最后打包好的文件就可以给电脑去判读执行了。
>
>————维基百科

简单来说，编译器能将你写的高级语言代码编译成机器语言，以此来达到 “运行程序” 的目的。

编译器的例子：GCC/G++, Microsoft Visual C++(简称vc,msvc)


### 集成开发环境 (IDE)

>集成开发环境（Integrated Development Environment，简称IDE，也称为Integration Design Environment、Integration Debugging Environment）是一种辅助程序开发人员开发软件的应用软件，在开发工具内部就可以辅助编写源代码文本、并编译打包成为可用的程序，有些甚至可以设计图形接口。
>
>IDE通常包括编程语言编辑器、自动构建工具、通常还包括调试器。有些IDE包含编译器／解释器，如微软的Microsoft Visual Studio，有些则不包含，如Eclipse、SharpDevelop等，这些IDE是通过调用第三方编译器来实现代码的编译工作的。有时IDE还会包含版本控制系统和一些可以设计图形用户界面的工具。许多支持面向对象的现代化IDE还包括了类别浏览器、物件查看器、物件结构图。虽然目前有一些IDE支持多种编程语言（例如Eclipse、NetBeans、Microsoft Visual Studio），但是一般而言，IDE主要还是针对特定的编程语言而量身打造（例如Visual Basic、Spyder）。
>
>————维基百科

大概可以认为是一个同时携带了编辑器、编译器等的程序，集成了编辑、文件、管理、编译、调试、执行等功能。大部分老师推荐的写代码的工具都属于这一类，使用便捷、功能强大。

集成开发环境的例子：DEV C++, Visual Studio, Pycharm, Eclipse, Codeblocks

# 正文

## Visual Studio Code：或许是你的第一选择

>Visual Studio Code（简称VS Code）是Microsoft在2015年4月30日Build开发者大会上正式宣布的一个运行于 Mac OS X、Windows和 Linux 之上的，针对于编写现代Web和云应用的跨平台源代码编辑器， 可在桌面上运行，并且可用于Windows，macOS和Linux。它具有对JavaScript，TypeScript和Node.js的内置支持，并具有丰富的其他语言（例如C++，C＃，Java，Python，PHP，Go）和运行时（例如.NET和Unity）扩展的生态系统。
>
>————百度百科

诞生于2015年的 VSCode 编辑器，现在可以说是目前最强的编辑器之一，在微软的背景下，比各位历史悠久的老大哥成长快得多，经过不到5年的时间便坐到了市场占有率第一的位置。这么短的时间里，它是怎么成功的？答案是：**简单，可扩展性强**。

编辑器，简单很重要。一个工具的学习曲线会直接影响该工具的受众数量，对于编辑器而言尤其如此。对于我们在桌面端编程而言，越简单好用的编辑器越好，不要搞骚操作，最终烦的是自己。这就是为什么 VSCode 越来越火爆，而且它不仅简单易用，还能覆盖几乎所有语言的编写，如果我有一个小项目需要涉及到前后端所有代码，用 VSCode 一个编辑器就能解决了，而不是前端切 Webstorm，后端切 Pycharm。

如果你是刚学代码刚刚会写 hello world 的新手玩家，你可以很顺手的用它来写你的C语言数学题。如果你是业界大拿，纯 Vim 开发，也完全支持。真正的用户，更多的是日常在开发的普通软件工程师，一样配合各种插件就能很方便的完成日常的工作。

VSCode 不仅仅是一个代码编辑器，它靠强大的生态，可以满足你各种各样的需求。不论什么语言，只要装上插件就能有基础 IDE 的功能。不论什么水平，只要简单操作，就能完全搭配好适合自己的开发模式。

极度灵活的编辑器，如果你什么也不装，它就像一把安安静静的 .22手枪；如果你装上需要的插件，它就是一把能扫穿香蕉道的 Negev。

为什么大家都喜欢用呢？主要的原因是学习曲线非常友好，新手上手使用极快。同时，借助开源，功能方面社区一直都有在跟进，再加上大量的插件构成的生态，组成了这样的极其灵活的开发环境。

## 

## Visual Studio：与 VSCode 的对比

| | VS | VSCode |
| --- | --- | --- |
| 功能 | Visual Studio 是一种集成开发环境，也称为 IDE|	Visual Studio Code 是一个代码编辑器，开发人员可以轻松地编辑他们的代码|
| 运行速度 |在跨不同平台执行时，VS 速度较慢。处理速度较慢| VS Code 相对较快 |
| 定价 |Visual Studio 有一个免费的编辑器供开发人员使用，但也提供了更好的付费 IDE 版本。|	VS Code 完全免费并且是开源的|
| IntelliSense功能 | VS 采用最好和最先进的 IntelliSense | IntelliSense 在 VS Code 中相对不合格 |
| 存储需求 | 整体下载大小相当大，占用大量存储空间 |	与 Visual Studio 相比，Visual Studio Code 非常轻量级，它不需要大量存储空间或大量下载 |
| 内存需求 |VS 需要更多内存才能更好、更流畅地工作 | VS Code 相对来说不需要很多空间来运行，它可以轻松地在 300 MB 的内存上运行 |
| 跨平台能力 |Visual Studio 仅在 macOS 和 Windows 上运行 |	VS Code 可以在 macOS、Windows 和 Linux 上运行 |
| 拓展性 | 没有多少专业开发的插件可用于 Visual Studio |	VS Code 附带了广泛的专业策划插件和扩展，生态丰富，以满足各种编辑和编译需求 |


在我看来，VSC 是更适配大部分大学生的应用场景的，而 VS 更适合则局限在了某些特定语言 (C++, C#) 的专业的软件开发场景。


有人认为 VSC 需要**折腾**是 VSC 的缺点，但换个角度来看，这或许也是 VSC 的优点之一，折腾工具、搭建环境的过程中可以学到很多有用的东西，这是与计算机交流的过程，也是每一个进入代码世界的人的必经之路。事实上，Visual Studio 在很多时候比 Visual Studio Code 更为**折腾**，每次你都要为了创建一个 .c 文件而创建一整个解决方案，当你想创建一个 .c 源文件时你甚至还要把 .cpp 的后缀名改成 .c 才能开始开始写代码，这实际上才是最麻烦的部分。

>当然，这并不是说Visual Studio是一个不好的工具，它在很多方面都是非常优秀的，只是对于大学生来说，可能不是最适合的学习工具。
>———— NewBing

## JetBrains 全家桶等别的开发环境

没用过，不评价（纯fw）。

>所以你整到最后原来就用过这几个开发环境？那你推荐个毛线啊！

咳咳，只要知道 VSCode 好用就行啦，别的你自己去试试嘛，我刨去高中学了两年的 Python，连半年的代码经验都没有呢(

## 不推荐

### DEV C++

虽然类似蓝桥杯的编程竞赛使用的 IDE 是 DEV C++，但是我还是认为你不应该使用这个已经停更7年的老古董。

- DEV C++ 是一个已经停止更新多年的 IDE，功能和界面都非常落后，无法支持现代的C++语言特性和标准库，缺乏实时的代码补全、错误提示、重构等功能，对于提高编程效率和质量没有帮助

- DEV C++ 的除错器（Debugger）功能非常弱，经常出现无法正常运行或者显示错误信息的情况，对于初学者来说，很难找到自己代码中的问题，也无法深入理解程序的运行过程和原理

### VC 2010

伙计，你应该知道现在是2023年，不是2013年！

### Python IDLE

虽然你高中可能用这玩意写了两年的 Python，但是我还是建议你忘了它吧，你还不如把它当作一个没汉化过的记事本。

# Todo

lots of~

# 参考资料

- [挑把趁手的兵器——VSCode配置C/C++学习环境（小白向）](https://zhuanlan.zhihu.com/p/147366852)
- [为什么好多编程“牛人”不喜欢用 Microsoft Visual Studio？](https://www.zhihu.com/question/30589163)
- [Python 编程的最好搭档—VSCode 详细指南](https://zhuanlan.zhihu.com/p/112431369)
- [Visual Studio和Visual Studio Code(VSCode)的区别及如何选择-前端开发自学笔记(7)](https://zhuanlan.zhihu.com/p/565412998)
- [把VS Code打造成后端开发的宇宙IDE，也挺爽！](https://zhuanlan.zhihu.com/p/437236290)