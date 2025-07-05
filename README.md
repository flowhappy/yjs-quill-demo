```new WebsocketProvider('ws://localhost:1234', 'quill-demo-room', ydoc);```的```ws://localhost:1234```是搭建的服务器地址

## 搭建y-websocket服务器

新建一个文件夹，在这个文件夹里的控制台里面：

第一步：安装并启动 @y/websocket-server
  ```npm install @y/websocket-server ```
  以下的代码要逐行运行
```
set HOST=localhost
set PORT=1234
npx y-websocket
```
服务器搭建完成，可以实现协同编辑功能
