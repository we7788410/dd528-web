# 文档结构说明

## 项目文档结构

项目使用nodeJS搭建，文档整体的结构符合node的常规结构。

* config：配置文件的目录，用于存放不同环境(development-开发、production-生产)的配置信息，因是开源项目，所以不存在测试环境
* doc：文档信息，用于存在整个项目中需要单独说明、总结的一些文档
* public：公用文件文件夹，用于存放整个项目中公用的资源文件，类似于src
    * static：静态资源文件夹，用于存放整个项目中用到的静态资源，主要包括历史版本记录、更新日志等
        * history.json：版本历史记录文件，记录开发中的迭代版本，每个版本的更新内容和技术说明、创建时间等信息
* router：路由文件文件夹，用于存放控制整个项目中路由的文件
* test：测试文件文件夹，用于存放测试文件，某个新技术的测试使用
* service：服务文件文件夹，用于存放抽象到service层的原子性（最小不可分割的request代码单元）代码
* utils：工具类文件夹，用于存放公用调用的方法类
* views：视图层文件文件夹，使用ejs模板，用于存放ejs模板的资源文件
* .gitignore：git的ignore文件列表
* app.js：启动文件，node app.js即可启动本项目，具体内容见内部注释
* LICENSE：遵循的协议说明，本开源项目遵循MIT协议，具体协议内容见[本文件](./LICENSE)
* package.json：项目说明，内容包含整个项目使用的module的版本信息及项目的整体信息
* README.md：git的起始文件，每个文件夹下的README.md即为git路径打开时的预览内容，内部包含整个文件夹的说明信息

## doc中文档结构