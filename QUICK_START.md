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

必须切换到`src/proxy-server/`目录再执行，否则可能报错：https://github.com/JSREI/ast-hook-for-js-RE/issues/27

```
cd src/proxy-server/
node proxy-server.js
```

访问 http://localhost:8002/ 地址，安装https证书

启动服务

```
node src/api-server/api-server.js
```


最后在浏览器中将代理设置为 http://127.0.0.1:10086 即可。


## 使用示例

访问 https://www.xiniudata.com/

在 console 找到 https://www.xiniudata.com/api2/service/x_service/person_home/list_home_tag_company 这个请求，找到sig的值。

在consloe调用hook.search方法，使用sig的值搜索，即可找到对应的代码。

```
hook.search("your sig value")
```
