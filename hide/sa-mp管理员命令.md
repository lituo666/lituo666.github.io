---
title: sa-mp管理员命令
date: 2019-02-18 15:22:30
tags:
- GTA-SA
  - SAMP
  - SAMP-笔记
categories: GTA-SA
---

# RCON命令

## 使用方法

> 1、可以直接在服务器端的命令窗口输入命令，不用加`/rcon`
> 2、在命令窗口输入`'/rcon login password`，其中`password`是`server.cfg`中`rcon_password`字段设置的密码

## 所有RCON命令 

<!--more-->

<table><tr><th width='16.59%'>命令</th><th width='46.65%'>机器翻译</th><th width='36.76%'>原文</th></tr><tr><td>/rcon cmdlist </td><td>显示所有命令。</td><td> Shows a list with commands.</td></tr><tr><td>/rcon varlist </td><td>显示包含当前变量的列表。</td><td> Shows a list with the current variables.</td></tr><tr><td>/rcon exit </td><td>关闭服务器。</td><td> Closes the server.</td></tr><tr><td>/rcon echo [text] </td><td>显示服务器控制台中的[text]（不是游戏中的客户端控制台）</td><td> Shows the [text] in the console of the server (NOT the client_console in game).</td></tr><tr><td>/rcon hostname [name] </td><td>更改主机名文本（例如：/ rcon hostname my server）</td><td> change the hostname text (example: /rcon hostname my server).</td></tr><tr><td>/rcon gamemodetext [name] </td><td>更改gamemode文本（例如：/ rcon gamemodetext my gamemode）</td><td> change the gamemode text (example: /rcon gamemodetext my gamemode).</td></tr><tr><td>/rcon mapname [name] </td><td>更改地图名称文本（例如：/ rcon mapname San Andreas）</td><td> change the map name text (example: /rcon mapname San Andreas).</td></tr><tr><td>/rcon exec [filename] </td><td>执行包含服务器cfg的文件（例如：/ rcon exec blah.cfg）</td><td> Executes the file which contains server cfg (example: /rcon exec blah.cfg).</td></tr><tr><td>/rcon kick [ID] </td><td>使用给定的ID踢出玩家（例如：/ rcon kick 2）</td><td> Kick the player with the given ID (example: /rcon kick 2).</td></tr><tr><td>/rcon ban [ID] </td><td>禁止具有给定ID的玩家（例如：/ rcon ban 2）</td><td> Ban the player with the given ID (example: /rcon ban 2).</td></tr><tr><td>/rcon changemode [mode] </td><td>此命令将当前游戏模式更改为给定的游戏模式（例如：如果要播放sftdm：/ rcon changemode sftdm）</td><td> This command will change the current gamemode to the given one (example: if you want to play sftdm: /rcon changemode sftdm).</td></tr><tr><td>/rcon gmx </td><td>将加载server.cfg中的下一个游戏模式。</td><td> Will load the next gamemode in server.cfg.</td></tr><tr><td>/rcon reloadbans </td><td>重新加载存储禁止的IP地址的samp.ban。应在取消和IP地址后使用。</td><td> reloads the samp.ban where the banned IP addresses are stored. Should be used after unbanning and IP address.</td></tr><tr><td>/rcon reloadlog </td><td>重新加载server_log.txt。对任何事情没有明显影响。</td><td> reloads the server_log.txt. Has no noticeable effect on anything.</td></tr><tr><td>/rcon say </td><td>在client_console中向玩家显示一条消息（例如：/ rcon表示hello将显示为* Admin：hello）</td><td> shows a message to the players in the client_console (example: /rcon say hello will show as * Admin: hello).</td></tr><tr><td>/rcon players </td><td>显示服务器中的播放器（带有名称，IP和ping）</td><td> Shows the players that are in the server (with their name, IP & ping).</td></tr><tr><td>/rcon banip [IP] </td><td>禁止给定IP（例如：/ rcon banip 127.0.0.1）</td><td> Ban the given IP (example: /rcon banip 127.0.0.1).</td></tr><tr><td>/rcon unbanip [IP] </td><td>取消给定的IP（例如：/ rcon unbanip 127.0.0.1）</td><td> Unban the given IP (example: /rcon unbanip 127.0.0.1).</td></tr><tr><td>/rcon gravity </td><td>改变重力（例如：/ rcon gravity 0.008）</td><td> Changes the gravity (example: /rcon gravity 0.008).</td></tr><tr><td>/rcon weather [ID] </td><td>改变天气（例如：/ rcon weather 1）</td><td> Changes the weather (example: /rcon weather 1).</td></tr><tr><td>/rcon loadfs </td><td>加载给定的filtercript（例如：/ rcon loadfs adminfs）</td><td> Loads the given filterscript (example: /rcon loadfs adminfs).</td></tr><tr><td>/rcon weburl [server url] </td><td>更改masterlists / SAMP客户端中的服务器URL</td><td> Changes the server URL in the masterlists/SAMP client</td></tr><tr><td>/rcon unloadfs </td><td>卸载给定的filterscript（例如：/ rcon unloadfs adminfs）</td><td> Unload the given filterscript (example: /rcon unloadfs adminfs).</td></tr><tr><td>/rcon reloadfs </td><td>重新加载给定的filtercript（例如：/ rcon reloadfs adminfs）</td><td> Reloads the given filterscript (example: /rcon reloadfs adminfs).</td></tr><tr><td>/rcon rcon_password [PASSWORD] </td><td>更改rcon的密码</td><td> Change the rcon's password</td></tr><tr><td>/rcon password [password] </td><td>设置/重置服务器密码</td><td> Sets/resets the server password</td></tr></table>

---

> 以下命令仅使用于0.3z R2 及以上：		

<table><tr><th width='20.91%'>命令</th><th width='46.67%'>机器翻译</th><th width='32.39%'>原文</th></tr><tr><td>/rcon messageslimit [count] </td><td>更改客户端每秒发送到服务器的消息数（默认500）</td><td> Change the number of messages per second a client sends to the server. (default 500)</td></tr><tr><td>/rcon ackslimit [count] </td><td>更改确认限制（默认为1000）（因为0.3z R2_2，默认限制为3000）</td><td> Change the limit of acks (default 1000) (Since 0.3z R2_2, default limit is 3000)</td></tr><tr><td>/rcon messageholelimit [count] </td><td>更改消息孔的限制（也可在0.3z R1中使用）（默认为3000）</td><td> Change the limit of message holes (Also available in 0.3z R1) (default 3000)</td></tr><tr><td>/rcon playertimeout [limit m/s] </td><td>更改时间（以毫秒为单位），直到播放器在未发送任何数据包时超时（默认1000）</td><td> Change the time in milliseconds until a player timeouts when not sending any packets. (default 1000)</td></tr><tr><td>/rcon language [language] </td><td>更改服务器语言（例如：/ rcon language English）。显示在服务器浏览器中。</td><td> Change the server language (example: /rcon language English). Shown in server browser.</td></tr></table>





