---
title: "{{ replace .Name "-" " " | title }}" # 文章标题
date: {{ .Date }} # 自动添加日期信息
draft: true # 设为false可被编译为HTML，true供本地修改
categories: [""] #文章类型，用于归档
tags: [""]  # 文章标签，可设置多个，用逗号隔开。Hugo会自动生成标签页
---

