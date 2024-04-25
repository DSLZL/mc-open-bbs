---
post: true
title: Dominion - 新的领地插件，支持Folia！
# 文章发布时间
date: 2024-04-23
# 文章LOGO的uri地址
cover: https://ssl.lunadeer.cn:14437/i/2024/04/23/662729db7fd3f.png
# 文章类目
categories:
    - 服务端插件
# 文章标签可多个
tags:
    - 搬运插件
# 文章的简介
description: 新的领地插件，支持Folia！
---


<div style="text-align: center;">

<img src="https://ssl.lunadeer.cn:14437/i/2024/03/28/6604f0cec0f0e.png" alt="" width="70%">

### [开源地址](https://ssl.lunadeer.cn:14446/zhangyuheng/Dominion) | [文档地址](https://ssl.lunadeer.cn:14448/doc/23/)

### [下载页面](https://ssl.lunadeer.cn:14446/zhangyuheng/Dominion/releases)

### [统计页面](https://bstats.org/plugin/bukkit/Dominion/21445) | [Hangar](https://hangar.papermc.io/zhangyuheng/Dominion)

</div>

## 简介

鉴于 Residence 插件的作者项目较多，维护压力大，无法及时跟进新版本以及适配Folia核心。故开发此插件，旨在平替纯净版生存服Residence的使用。

请注意，本插件仍然处于测试阶段，因此可能存在一定的行为控制漏洞。如果遇到此类遗漏的行为控制欢迎即使发送邮件或添加QQ告知，感激不尽。

## 说明

本插件基本还原了Residence的核心功能，主要适用于原版纯净生存服务器的防破坏目的，因此暂不考虑引入价格系统、商店等非原版Minecraft玩法。

![](https://ssl.lunadeer.cn:14437/i/2024/02/16/65cf3b08c986b.png)

为了提高存储效率，本插件使用了数据库+缓存的方式存储领地数据，玩家配置领地权限直接修改数据库内容，随后触发缓存更新。权限控制则以异步的方式访问缓存，减少事件阻塞。

权限系统主要由领地权限、玩家特权组成，玩家特权优先级高于领地权限。没有特权的玩家在领地内收到领地权限的控制，有特权配置则按照特权设置受控。

## 功能介绍

- 支持 Postgresql 或 sqlite 存储数据；
- 支持BlueMap卫星地图渲染；
- 支持为玩家单独设置特权；
- 支持设置领地管理员；
- 支持子领地；
- 采用 TUI 方式进行权限配置交互，简单快捷；

## 支持版本

- 1.20.1+ (Paper、Folia)

## TODO

- WebUI
- Admin TUI

## 建议与反馈

Mail: [zhangyuheng@lunadeer.cn](mailto:zhangyuheng@lunadeer.cn)

QQ群：309428300
