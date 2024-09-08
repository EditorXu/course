---
title: 讲义编写
icon: lightbulb
dir:
  link: true
---

## Markdown

Markdown**半小时**就能速成，类似word，但是比word简单很多，讲义需要用Markdown编写。我们会最基础的语法就行了。

::: important 学习Markdown
 - 所有人都要会 [Markdown速成](https://theme-hope.vuejs.press/zh/cookbook/markdown/)
 - 如果你想要更好的展示效果，可以参考[Markdown](https://theme-hope.vuejs.press/zh/guide/intro/markdown.html)
:::

## VuePress

如果你想维护网站，可以学习VuePress

VuePress**几小时**就能速成，因为我们直接用别人写好的东西，我们不需要**写**一个功能，只需要**开启**一个功能

::: tip 参考资料
Vuepress
  - [Vuepress](https://vuepress.vuejs.org/zh/guide/introduction.html)
  - [VuePress Theme Hope](https://theme-hope.vuejs.press/zh/get-started/)

如果你想让网站有质的突破，可以系统学习Web
  * [Web入门](https://developer.mozilla.org/zh-CN/docs/Learn/Getting_started_with_the_web)
  * [Vue](https://cn.vuejs.org/guide/introduction.html)
:::

## 本地构建
1. 下载[docker](https://docs.docker.com/engine/install/ubuntu/)

2. fork[网站](https://github.com/cyh834/course)到自己的github

3. clone刚才fork的存储库

4. 进入本地存储库
``` bash
cd course
``` 
5. 本地构建网站
``` bash
make test
```

`make test`会自动拉取镜像，如果因为网络问题导致镜像拉取失败，可以从[网盘](https://pan.baidu.com/s/1cP9hpwoIzC3cceHBG-aRkA?pwd=9wct)中下载

然后运行
``` bash
docker load -i web.tar
```
最后再次尝试`make test`

6. 用浏览器打开:[http://localhost:8080/course/](http://localhost:8080/course/)


## 修改讲义
1. 增加/修改`src/software`下的markdown文件
2. 然后`make test`

## 提交讲义

为了防止你们提交后网站挂了，请提[PR](https://blog.csdn.net/qq_33429968/article/details/62219783)