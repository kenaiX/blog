title: "工作技巧"
date: 2015-03-06 01:57:18
tags: work skill
---
此文档会保持更新，以Q&A方式收集工作的一些经验。

Q:工作中最长用到的工具？

A:git oh-my-zsh+autojump 印象笔记 chrome浏览器 android-studio

Q:习惯了用vim来写git commit记录，但是ubuntu默认用nano，怎么办？

<!-- more -->

A:~/.zshrc 中添加 echo export EDITOR="/usr/bin/vim"

Q:mac邮件客户端乱码：

A:内容处加一个'⌘'（放到签名里就可以了）。原理：加入此符号后会默认转码成UTF-8。

Q:git clone 等待时间过长？

A:git clone --depth=1 git@xxx.xxx:xxx，这样就会只获取最新的版本。（git fetch --unshallow 可以拉取所有版本记录）

Q:为什么建议用python取代bash脚本？

A:在不同文件系统下，bash脚本无法通用。例如在windows下用cygwin模拟linux环境的时候，bash就秀逗了。但是可以使用python简本执行 --> import os   os.system("bash command")

Q:Ubuntu下的工具推荐？

A:rsync，screen，

Q:JAVA7中增强数字的可读性？

A:1000000.0000 --> 1000_000.000_0

