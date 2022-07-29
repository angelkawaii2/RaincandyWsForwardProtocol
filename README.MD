# Raincandy Websocket-Forward Protocol

A Websocket-based forward protocol.

一个基于 Websocket 的数据转发协议库的项目

如需编译子项目，请 ``clone`` 本仓库后，运行

```bash
git submodule update --init --recursive
```

之后在本仓库目录下使用 gradle 进行编译.

## 工作原理

本程序为CS架构，其中 Client 连接到 Server 后，封装需要传输的信息（目标Client ID、消息本体等），然后通过 Websocket 发送给
Server。
Server 端收到消息后，判断消息目的地，将其转发给目标 Client。

## 子模块列表/Submodules List

> 点击可直接跳转到对应仓库

### [WSFProtocolSDK](https://github.com/angelkawaii2/WSFProtocolSDK/)

Provide SDK for all other modules.

项目 SDK，其他子模块需依赖此部分

### [WSFMiraiForwardPlugin](https://github.com/angelkawaii2/WSFMiraiForwardPlugin)

The plugin of Mirai-console.

Mirai-console 的插件实现

### [WSFSpigotForwardPlugin](https://github.com/angelkawaii2/WSFSpigotForwardPlugin)

The plugin of SpigotMC.

Bukkit/Spigot插件实现

### [WSFFabricForwardMod](https://github.com/angelkawaii2/WSFFabricForwardMod)

The mod of Fabric.

Fabric端模组实现（server）

### [WSForwardServer]()

Server端（暂未实现）
