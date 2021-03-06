---
title: "Hello Hugo" # 文章标题
date: 2019-04-20T01:50:56+08:00 # 自动添加日期信息
draft: true # 设为false可被编译为HTML，true供本地修改
categories: ["工具~技巧"] #文章类型，用于归档
tags: ["博客","Hugo"]  # 文章标签，可设置多个，用逗号隔开。Hugo会自动生成标签页
---

### Hello Hugo

Hugo 是由 Go 语言实现的静态网站生成器。简单、易用、高效、易扩展、快速部署。

- 官网：https://gohugo.io
- 中文文档：https://www.gohugo.org

```css
Have fun!
```

---------

Hugo is the world’s fastest framework for building websites. It is written in Go.

It makes use of a variety of open source projects including:

- https://github.com/russross/blackfriday
- https://github.com/alecthomas/chroma
- https://github.com/muesli/smartcrop
- https://github.com/spf13/cobra
- https://github.com/spf13/viper

Learn more and contribute on GitHub.

------



## 关于博客主题：LeaveIt

- Github链接:https://github.com/liuzc/LeaveIt

- 中文说明：https://liuzhichao.com/2018/hugo-theme-leaveit/

### 部署过程中遇到的问题

1. 使用该主题时，文章标题*号后面要加空格，如：二号标题写法为：`**空格+内容`

2. TODO：文章目录导航(待添加)，可参考：https://github.com/liuzc/LeaveIt/pull/11

3. TODO: 使用Travis CI 自动部署Hugo博客，https://mogeko.me/2018/028/

    

    

### 部署命令：

   进到`~/Documents/OneDrive/hugo_blog/blog-hugo/mysite`目录,执行如下git命令：

   ```css
   hugo --theme=LeaveIt --buildDrafts --baseUrl="https://topsee.top"
   ```

   --buildDrafts 不加会生成无内容的网站

   --baseUrl要和config.toml的地址一致。

​    

   顺利的话会创建public文件（里面的内容就是你要上传的静态网站的文件。）

   ```css
   cd public
   git status
   git add -A
   git commit -m "first commit"
   git push -u origin master
   ```

   如果push报错，尝试执行如下命令后再次push：

   ```css
   git pull origin master --allow-unrelated-histories
   ```

   

### 写作工具

1. Markdown工具：[Typora](https://www.typora.io)

2. 图床：[聚合图床](https://www.superbed.cn)和[SM.MS](https://sm.ms)(已弃)。测试一下：![](https://pic.superbed.cn/item/5cc4ff583a213b0417258690)

3. 图片压缩：[tinypng](https://tinypng.com)

4. 图片上传工具：待续

