---
layout: post
title:  如何在termux中安装Elixir
date: 2018-10-23 11:04 +0800
description: termux
img: post-6.jpg # Add image post (optional)
tags: [Erlang,Elixir]
author: bushrose
other: true
---

1. 安装`Erlang`
> apt install erlang
2. 下载![Elixir](https://elixir-lang.org/install.html)官网预编译的文件。

> `wget https://github.com/elixir-lang/elixir/releases/download/v1.7.3/Precompiled.zip
`
3. 解压下载的压缩包。
> `unzip Precompiled.zip -d elixir`

-d 指定解压的目录。若出现`command not found`，请安装unzip。
> `apt install unzip`
4. 添加文件内`bin`的路径到`PATH`。
> `vim .bashrc`</br>
`export PATH=$PATH:~/elixir/bin`

保存文件退出。然后执行`source .bashrc`让配置立即生效。

5. 检查安装是否成功。</br>
执行`iex`，若出线iex的REPL(交互式命令解释器)，则安装成功。
