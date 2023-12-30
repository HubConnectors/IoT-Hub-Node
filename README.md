# IoT-Hub-Node 

![](./logo.png)

用不同的语言阅读：[English](./README-EN.md) | [简体中文](./README.md) | [繁体中文](./docREADME-CHT.md)

## 介绍

IoT-Hub-Node是一个基于 Node.js 的物联网设备接入管理平台，旨在连接物联网设备和应用程序。它提供了一系列基于 HTTP 的API，用于设备管理、消息发送和接收，以及查询设备注册表和元数据。此外，它还提供了基于 MQTT 的硬件接口，用于设备与物联网的连接(这部分使用开源的MQTT服务器:[EMQX](https://github.com/emqx/emqx)来实现)。未来，我们还计划开发其他接口，例如基于 Websocket 的接口，以提供更多选择。

使用 Node.js 进行开发，可在云端或本地部署，并能在不同平台上运行，如 Windows、Linux、MacOS 等。使用 MySQL 作为默认数据库，并采用 Sequelize 作为 ORM 框架，这使得用户在需要切换数据库时非常方便。此外，Node.js 的异步非阻塞特性也使得其能够处理大量并发请求，具备高效处理能力。

通过优化和不断改进，IoT-Hub-Node 可以支持各种物联网应用程序的开发，例如智能家居、智能工厂和智能农业等领域。它提供了强大的功能和灵活性，使得开发人员能够构建出高性能、可靠的物联网应用程序。

目前，IoT-Hub-Node还处于开发阶段，后续会逐步完善功能。

## 初衷

本项目的初衷有两个主要目标：

1. 记录个人学习 node.js 的过程：在开发日志中详细记录学习过程中遇到的问题和解决方案，希望能够帮助其他人。

2. 提供一个基于 node.js 的物联网设备管理平台：实现设备管理、消息发送和接收，查询设备注册表和元数据等功能。希望通过这个平台让没有物联网开发经验的开发者能够快速开发物联网应用程序，并让前端开发者更轻松地接触物联网领域。我们希望通过这个项目，让物联网开发者和嵌入式开发者能够更容易地接触物联网，体会 web 技术在嵌入式领域的使用。


## 当前状态
我当前是一名学生，由于我的专业是电气工程及智能控制，对于 web 开发并不熟悉。在学习物联网领域时，我遇到了很多困难。因此，通过这个项目，我希望能够帮助其他人更轻松地开发和理解物联网应用程序。

我会在开发日志中记录学习过程中遇到的问题和解决方案，并在我的个人博客上发布一些学习笔记。你可以在[DuRuofu的个人博客](https://www.duruofu.xyz/)找到这些内容。我将以一个初学者的角度开始这个项目，并欢迎你在 issue 中提出你的想法。我会尽可能完善这个项目。

如果你对这个项目感兴趣，欢迎加入我们一起开发。我们欢迎你提供建议和帮助。

您想贡献吗？阅读我们的[贡献指南](./docs/CONTRIBUTING.md)以了解更多信息。有很多方法可以提供帮助！😃

## 项目结构

下面是项目的项目结构示意：

```
- controllers       // 控制器，处理路由逻辑
- models            // 数据模型，数据库交互
- services          // 业务逻辑层，处理复杂业务
- middlewares       // 中间件，请求预处理逻辑，例如权限验证
- routes            // 路由定义
- config            // 配置文件夹
- utils             // 工具函数或类
- public            // 静态资源文件夹
- routes            // 路由文件夹
- logs              // 日志文件夹
- tests             // 测试文件夹
- seeders           // 存储种子文件，用于向数据库表添加测试数据
- migrations      //存储的是迁移文件，用于数据库及数据库表的更新
- docs              // 文档目录
   - CONTRIBUTING.md   // 包含关于如何为项目做出贡献的准则和说明。
   - API.md            // 包含项目的应用程序编程接口（API）的文档。
   - TUTORIAL.md       // 一个教程，提供关于如何使用项目的详细指南。
   - DESIGN.md         // 项目的设计文档，描述了项目的架构、组件、数据流和交互过程等细节。
- .gitignore        // git忽略文件
- package.json      // 项目配置文件
- app.js            // 入口文件
- README.md         // 项目的入口文件，通常提供项目的概述、背景信息、安装指南、使用说明和贡献指南等信息。

```


以及[设计文档](./docs/DESIGN.md)|[开发日志](./docs/DEVELOPMENT_LOG.md)等文档。


## 开始使用

参考[快速开始](./docs/TUTORIAL.md)以了解如何在本地运行项目。

详细内容请参考[API文档](./docs/API.md)

## 更新日志


详细版本更新日志记录在[更新日志](./docs/CHANGELOG.md)中。

## 后续计划
关于项目开发计划记录在[开发日志](./docs/TODO.md)中。


## 联系我
如果你想了解更多关于此项目的信息,请阅读[设计文档](./docs/DESIGN.md),[开发日志](./docs/DEVELOPMENT_LOG.md).或者通过邮箱联系我: [duruofu@qq.com]