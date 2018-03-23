[TOC]

# eclipse配置手顺

## windows10 任务栏有多个图标，锁定任务栏失败

在eclipse目录下，修改eclipse.ini文件，在-vmargs之前：

```
-vm
C:\Program Files\Java\jdk1.7.0_04\bin
```



## 代码自动补全

Windows --> Preference --> 搜索Content Assist

auto activation triggers for Java 填入

`abcdefghijklmnopqrstuvwxyz.`

![搜狗截图20180321162501](C:\Users\zhichao.feng\Desktop\worknotesMD\配图\搜狗截图20180321162501.jpg)

## keymap

Window --> Preference --> General --> Key

需要修改

- collapse -- ctrl + _
- collapse All -- ctrl + shift + _
- expand -- ctrl + +
- expand All -- ctrl + shift + +

![搜狗截图20180321162704](C:\Users\zhichao.feng\Desktop\worknotesMD\配图\搜狗截图20180321162704.jpg)

## 编辑器颜色修正

1. 大括号匹配

   Window --> Preference --> Java--> Editor

![搜狗截图20180321163614](C:\Users\zhichao.feng\Desktop\worknotesMD\配图\搜狗截图20180321163614.jpg)

2. 匹配代码高亮

   Window --> Preference --> General --> Editor --> Text Editors --> Annotations

   ![搜狗截图20180321164249](C:\Users\zhichao.feng\Desktop\worknotesMD\配图\搜狗截图20180321164249.jpg)

