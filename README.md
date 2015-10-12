
## 目录结构

```
.
├── public          // LeanEngine Web 前端发布目录，前端（HTML\CSS\JavaScript）构建后放在此目录中
├── server-modules  // 服务器端代码模块目录
│    ├── app.js            // LeanEngine 服务端代码主入口
│    ├── api-router.js     // API 接口路由配置
│    ├── tool.js           // 工具方法
│    └── hello.js          // 示例代码
├── web-project     // Web 前端项目目录
│    ├── gulp           // 自动化构建的逻辑模块
│    ├── dist           // 构建之后的源码目录
│    └── src            // 源码目录
└── server.js       // LeanEngine 的环境配置
```



### 依赖安装

* 首先 clone 这个代码库到本地目录中

* 再在该项目`根目录`执行
```
$ npm install
```
安装服务端环境依赖

* 在 `web-project 目录`中执行
```
$ npm install
```
安装 Web 端构建依赖

* 在 `web-project 目录`中执行
```
$ bower install
```
安装 Web 端基础库

### 调试

* 在根目录执行
```
$ avoscloud
```
运行服务器端环境，通过 `http://localhost:3000/api/hello` 可以测试

* 在 web-project 目录中执行
```
$ gulp serve
```
运行 web 端环境，通过 `http://localhost:9000` 可以调试

* 开发时需要同时运行这两个任务（开两个 terminal），就可以同时调试 Server 与 Web



