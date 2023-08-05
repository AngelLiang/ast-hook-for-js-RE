# 快速开始

1、安装
2、启动代理
3、安装证书
4、启动服务

## 详细步骤

安装

```
npm install 
```

启动代理

```
node src/proxy-server/proxy-server.js
```

访问 http://localhost:8002/ 地址，安装https证书

启动服务

```
node src/api-server/api-server.js
```


最后在浏览器中将代理设置为 http://127.0.0.1:10086 即可。
