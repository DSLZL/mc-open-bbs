---
post: true
title: 使用新版opl联机mc教程
date: 2024-04-23 16:05:39
cover: https://doc.mcbbs.top/logo.svg
categories:
    - 联机教程
tags:
    - 原创教程
description: 使用新版OPL联机工具联机MC的教程
---

本教程前提是你和你的朋友已经安装了相同版本，且mod相同的minecraft.

同时建议存在无正版玩家时，都使用外置登录

注意，此教程为面向小白的教程，可能内容写得过于详细，请自行判断是否需要阅读。

粘贴`ctrl` + `v`   复制`ctrl` + `c`

### 作为房主

1. 打开minecraft，进入游戏，选择单人游戏，根据情况进入世界
2. 点击`esc`(键盘左上角)，点击`对局域网开放`
3. 记录左下角出现的端口号
4. 双击运行软件主程序，从页面左上角获取你的UUID
5. 将你的`UUID`和`端口号`发个你的朋友，并点击右上角的启动按钮

![tp1](https://blog.gldhn.top/2024/04/22/opl_mc/tp1.png)

### 作为连接的玩家

1. 打开minecraft，点击多人游戏
2. 打开软件主程序，点击右上角`新建连接`
3. 依次输入房主为你提供的UUID和端口（填远程端口，本地端口会自动填写）协议选择`TCP`

    ![tp2](https://blog.gldhn.top/2024/04/22/opl_mc/tp2.png)

4. 点击添加，然后点击右上角的启动
5. 可以在隧道列表处看到你的连接，`连接：ip:端口 ->`后为你进游戏的ip地址（请完整复制）
    ![tp3](https://blog.gldhn.top/2024/04/22/opl_mc/tp3.png)
6. 观察等待隧道列表处状态灯变为绿色
7. 回到游戏，点击`添加服务器`输入第5点处获取的ip地址(可提前添加)

   ps：1.0.1.17版本开始单tcp隧道启用情况下连接成功后世界会出现在局域网，无须添加
8. 刷新服务器列表，出现服务器信息后双击进入世界

后续再次使用点击编辑更换`远程端口`为房主新的对外开放端口即可

### 常见问题

- 游戏显示`登入失败，无效的会话`：正版验证问题(房主登录了一般就不会出现)，都使用外置登录或加联机模组关闭验证即可（个人推荐外置登录，还能加载皮肤披风，以下为设置外置登录的方法）
  - pcl ：版本设置->设置->服务器->登录方式->第三方登录：AuthlibInjector或LittleSkin->设置为littleskin->返回主页注册或登录
  - hmcl ：账户 -> 选择littleskin(没有点下面添加认证服务器，填入`https://littleskin.cn/api/yggdrasil`) -> 注册或登录

### 后记

后续联机仅房主游戏对外开放端口会发生改变，房主发送新的端口即可，连接的玩家只需要点击编辑修改`远程端口`即可

隧道可自行选择是否启用，也可以点击编辑参数

opl联机工具下载地址：[UI版](https://blog.gldhn.top/2024/04/19/opl_ui/)
