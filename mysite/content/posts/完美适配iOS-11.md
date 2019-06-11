---
title: "完美适配iOS 11"
date: 2018-05-30T09:44:16+08:00
categories: ["编程~技术"]
tags: ["iOS 11"]
---


### 前言

> 升级iOS 11 之后，发现屏幕适配的bug   
> 以下为适配解决方案

#### 在`Appdelegate.m`中的`didFinishLaunchingWithOptions`方法中添加如下代码，就全局搞定了！

```objective-c
if (@available(ios 11.0,*)) {
        
        UIScrollView.appearance.contentInsetAdjustmentBehavior = UIScrollViewContentInsetAdjustmentNever;
        
        UITableView.appearance.estimatedRowHeight = 0;
        
        UITableView.appearance.estimatedSectionFooterHeight = 0;
        
        UITableView.appearance.estimatedSectionHeaderHeight = 0;
        
    }
```
