---
title: FiveM服务器基本配置(1)
date: 2019-02-21 09:09:35
tags:
  - FiveM server 
  - GTA5
categories: FiveM server
---

# 修改加载页面
修改图片和音乐

> 1、将FiveM服务器目录`cfx-server-data-master/resources/[test]`下的`keks`文件夹在原位置复制一份，任意修改文件夹名，不能有中文。

<!--more-->

<img src="https://i.imgur.com/e3l3zaU.jpg" title="复制的keks文件夹" />

> 2、在`keks-user`文件夹下，新建一个文件夹`music`，用来存放音频文件，建议使用`ogg`的音频文件，<a href="https://convertio.co/zh/mp3-ogg/">点击这里</a>将`mp3`文件转换为`ogg`文件。

<img src="https://i.imgur.com/k1PL0YS.jpg" title="添加的ogg文件" />

> 编辑`keks-user`文件夹中的`index.html`文件，我使用的`Notepad++`软件编辑的。
> 在第一个`<body>`标签下，添加如下代码：

    <audio id="Loading" autoplay loop >
        <source src="music/Loading-Give-It-Up.ogg" type="audio/ogg">
    </audio>
    <script>
        var vid = document.getElementById("Loading");
        vid.volume = 0.2
    </script>

根据实际文件名修改`Loading-Give-It-Up.ogg`

<img src="https://i.imgur.com/naTCtAt.jpg" title="加入的代码" />

> 修改加载时的图片。将`keks-user`文件夹中的`loadscreen.jpg`替换掉就可以，

> 用微软的`Edge`浏览器打开`index.html`就可以看到自己加的图片和听到自己加的音乐了。
> 如果使用`Chorme`或者`IE`浏览器打开可能听不到声音。

> 编辑`keks-user`文件夹中的`__resource.lua`文件，在其中加入音乐文件的路径，如下图：

<img src="https://i.imgur.com/w7t69kO.jpg" title="加入音乐文件路径" />

> 最后在服务器配置文件`server.cfg`中添加资源名称'start keks-user'如下图：

<img src="https://i.imgur.com/VAyH7CK.jpg" title="在服务器配置中添加资源名称" />

