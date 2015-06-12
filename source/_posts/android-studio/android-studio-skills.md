title: "Android Studio 使用技巧"
date: 2015-03-11
categories: android
tags: work skill
---
此文档会保持更新

## 基础配置篇

* Appearance & Behavior --> Appearance --> Theme : Darcula

* Editor --> Colors & Fonts --> Font --> Scheme -> Save As ... --> Editor Font --> 调整字体和大小

<!-- more -->

* Plugins ： 

    关闭：Google XXX / GitHub / Maven Integration / Subversion Integration / Terminal 
	
	原因是大部分的google系在平时很难链接上，github不如直接用git命令来得实在，Terminal也不如用更好的终端。

    安装： ace jump

    推荐给不喜欢用IdeaVim插件的同学使用，跳转非常方便。

* keymap :

    Close --> Alt + w / acejump --> `

	纯粹个人喜好。

## 加速器篇

> 我们都希望自己的IDE能更快，按照如下几步去尝试，应该能达到一个理想的水平。

#### 1、配置最新的jdk

观察bin/studio.sh 代码，发现如下部分：

````
# ---------------------------------------------------------------------# Locate a JDK installation directory which will be used to run the IDE.# Try (in order): STUDIO_JDK, JDK_HOME, JAVA_HOME, "java" in PATH.# ---------------------------------------------------------------------if [ -n "$STUDIO_JDK" -a -x "$STUDIO_JDK/bin/java" ]; then  JDK="$STUDIO_JDK"elif [ -n "$JDK_HOME" -a -x "$JDK_HOME/bin/java" ]; then  JDK="$JDK_HOME"elif [ -n "$JAVA_HOME" -a -x "$JAVA_HOME/bin/java" ]; then  JDK="$JAVA_HOME"else
XXXXXX
````

我们都知道java版本肯定越高越快！但是我们平时需要使用的java版本可能不是最新的。因此建议下载一个最新的jdk给studio用。所以在~/.zshrc 里配置了如下一行

    export STUDIO_JDK=/usr/local/share/jvm/java8

windows下同理把最新的JDK加入'STUDIO_JDK'环境变量即可。