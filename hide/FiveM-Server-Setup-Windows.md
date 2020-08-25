---
title: FiveM服务器搭建
date: 2019-02-25 13:51:31
tags: 
 - FiveM server
 - GTA5 
categories: FiveM server
---

玩GTA5都是想在游戏里“为所欲为”，我们可以装修改器和装几个MOD，这些方法我们可以在单机的时候玩，但是自己玩总归是有些无聊。我们也知道GTA5在线模式，但是因为装了修改器和MOD有可能被封号。
我需要一种办法，既能在游戏里“为所欲为”，又能和小伙伴们联机玩游戏，接下来我们就介绍搭建FiveM服务器。

<!--more-->

---

## 下载服务器文件

首先，介绍FiveM服务器官网：https://fivem.net/ 点击`Download server(non-commercial)`如下图所示:

<img src="https://s2.ax1x.com/2019/02/28/k7z0K0.jpg" alt="k7z0K0.jpg" border="0" title="点击方框" />

网页跳转至说明文档，如下图所示:

<img src="https://s2.ax1x.com/2019/02/28/kHSSZ8.jpg" alt="kHSSZ8.jpg" border="0" />

服务器可以运行在Windows或者Linux上，这里讲解安装在Windows服务器上（Linux服务器看[这里](https://lituo666.top)），在上图中其实已经写着安装步骤，如果是Chrome浏览器可以右键翻译成中文。接下来详细讲解每一步操作。

### 安装Visual C++组件

安装<a href="https://go.microsoft.com/fwlink/?LinkId=746572">Visual C++ redistributable 2017</a>或更高版本。点击即可下载，这个文件不大，下载速度很快，然后双击进行安装。

### 下载主要文件

点击<a href="https://runtime.fivem.net/artifacts/fivem/build_server_windows/master/">这里</a>，根据时间，选择最新的文件点击进行下载，然后解压文件，去下图所示:

<img src="https://s2.ax1x.com/2019/02/28/kHS1zR.jpg" alt="kHS1zR.jpg" border="0" />
<img src="https://s2.ax1x.com/2019/02/28/kHS5Ss.jpg" alt="kHS5Ss.jpg" border="0" />

### 下载资源文件

点击<a href="https://github.com/citizenfx/cfx-server-data">这里</a>，然后点击绿色按钮`Clone or download`再点击`Download ZIP`进行下载。如下图所示：

<img src="https://s2.ax1x.com/2019/02/28/kHSHmV.jpg" alt="kHSHmV.jpg" border="0" />

## 服务器配置

### 解压服务器主要文件

将[前面](#下载主要文件)下载的`server.zip`文件解压，如下图所示：

<img src="https://s2.ax1x.com/2019/02/28/kHpKnP.jpg" alt="kHpKnP.jpg" border="0" />

### 解压资源文件

将[前面](下载资源文件)下载的`cfx-server-data-master.zip`文件解压到服务器文件夹中去。如下图所示：

<img src="https://s2.ax1x.com/2019/02/28/kHpBAU.jpg" alt="kHpBAU.jpg" border="0" />

### 添加配置文件

点击[这里](https://docs.fivem.net/server-manual/setting-up-a-server/#server-cfg)，将代码全部复制，如下图所示：

<img src="https://s2.ax1x.com/2019/02/28/kHpI4e.jpg" alt="kHpI4e.jpg" border="0" />

进入`cfx-server-data-master`目录下，新建文本文档，修改后缀为`cfg`，打开文件，将刚刚复制的粘贴进去。
下面是详细的配置说明

```
# 一般情况下不用修改!
# 只有使用多个服务器协议的时候才需要更改。默认的TCP和UDP端口为30120
endpoint_add_tcp "0.0.0.0:30120"
endpoint_add_udp "0.0.0.0:30120"

# 默认启动资源。
start mapmanager
start chat
start spawnmanager
start sessionmanager
start fivem
start hardcap
start rconlog
start scoreboard
start playernames

# 允许玩家使用scripthook挂载的修改器，例如lambda菜单。
# 设置为0可以禁用。
sv_scriptHookAllowed 1

# 取消前面的#可以启动RCON，记住你更改的密码。
#rcon_password changeme			#一般用不到

# 服务器标签，中间用逗号隔开
# 例如：
# - sets tags "drifting, cars, racing"
# 或者：
# - sets tags "roleplay, military, tanks"
sets tags "default"

# 设置服务器横幅或者链接横幅的URL
# 大小没有限制，任何图像都可以.
#sets banner_detail "http://url.to/image.png"
#sets banner_connecting "http://url.to/image.png"

# 设置服务器名称
sv_hostname "My new FXServer!"

# 嵌套配置！一般不改。
#exec server_internal.cfg

# 服务器LOGO图标 (96x96 PNG文件)
#load_server_icon myLogo.png

# 可以在脚本中使用的封面。
set temp_convar "hey world!"

# #如果你不想服务器显示在FiveM网页服务器列表，可以把#号删掉。
#sv_master1 ""

# 只能让Steam或者第三方运营商进入你的FiveM服务器?
# 不要忘记Social Club也是第三方提供商!
# 一般不改
#sv_authMaxVariance 1
#sv_authMinTrust 5

# 添加系统管理员。
add_ace group.admin command allow # allow all commands
add_ace group.admin command.quit deny # but don't allow quit
add_principal identifier.steam:110000112345678 group.admin # add the admin to the group

# 在外部输出日志上不显示玩家的信息。
sv_endpointprivacy true

# 服务器人数设置 (必须在 1 到 32)
sv_maxclients 32

# 服务器密钥 (https://keymaster.fivem.net)
sv_licenseKey changeme


```

> 1、先在[FiveM论坛](https://forum.fivem.net/)注册账户。
> 2、再去获取[服务器密钥](https://keymaster.fivem.net)（打不开请挂代理）,服务器IP就是本机的IP,百度即可。如下图所示：
<img src="https://s2.ax1x.com/2019/03/01/kbFoKH.jpg" alt="kbFoKH.jpg" border="0" />
<img src="https://s2.ax1x.com/2019/03/01/kbFTrd.jpg" alt="kbFTrd.jpg" border="0" />
> 2、在`server.cfg`中填写服务器密钥。

### 添加服务器运行命令

进入服务器目录`FXServer`，新建一个文本文档，名称任意，将后缀改为`bat`然后右键编辑，添加如下代码：
```
cd /d F:\FXServer\cfx-server-data-master
F:\FXServer\run.cmd +exec server.cfg
```

> 说明
> 第一行`F:\FXServer\cfx-server-data-master`是资源文件夹，根据自己实际文件夹路径进行修改。
> 第二行`F:\FXServer`是服务器目录，根据实际修改；`server.cfg`是配置文件名。

## 启动服务器

双击刚刚新建的后缀为`bat`的文件，出现如下图说明启动成功。

<img src="https://s2.ax1x.com/2019/03/01/kbAiOH.jpg" alt="kbAiOH.jpg" border="0" />

