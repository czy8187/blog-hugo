---
title: "Mac系统下Homebrew关闭自动更新" # 文章标题
date: 2019-04-20T21:53:21+08:00 # 自动添加日期信息
draft: true # 设为false可被编译为HTML，true供本地修改
categories: ["工具 ~ 技巧"] #文章类型，用于归档
tags: ["Homebrew"]  # 文章标签，可设置多个，用逗号隔开。Hugo会自动生成标签页
---

在 mac 下使用 brew 安装软件时，默认每次都会自动更新 homebrew，显示
`$ Updating Homebrew…`,

网络状况不好或者没有换源的时候会很慢，卡在这里许久不动。
我们可以关闭自动更新，在命令行执行：

```css
$ export HOMEBREW_NO_AUTO_UPDATE=true
```

即可关闭自动更新。

<!-- more -->



如果想要重启后设置依然生效，可以把上面这行加入到当前正在使用的 shell 的配置文件中，比如我正在使用的是 zsh，在命令行执行以下语句：

```css
$ vi ~/.zshrc
```

然后在合适的位置，加入：

```css
# brew关闭自动更新
export HOMEBREW_NO_AUTO_UPDATE=true
```

