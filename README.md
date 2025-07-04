# 使用y.js做协同编辑

## 搭建客户端
按步骤操作
```npm create vite ```
```Ok to proceed? (y) y```
输入 Project name
framework choose ```Vanilla```
variant choose ```JavaScript```
```cd project-name```
```npm install```
``` npm run dev```

客户端搭建完成，```main.js```中```new WebsocketProvider('ws://localhost:1234', 'quill-demo-room', ydoc);```的```ws://localhost:1234```是接下搭建的服务器地址
到这一步已经实现了本地的协同编辑，同一个浏览器的不同标签页可以实现本地host的协同编辑，不同的浏览器则不可以

## 搭建y-websocket服务器
第一步：安装并启动 @y/websocket-server

    github文档说了：The fastest way to get started is to run the @y/websocket-server backend.
    (网页上的文档还没有更新，npx无效)
    并且提供了安装和启动的命令：
  ```npm install @y/websocket-server ```
  以下的代码要逐行运行
```
set HOST=localhost
set PORT=1234
npx y-websocket
```
服务器搭建完成，可以实现协同编辑功能
