# jackblog api express版

[![build status][travis-image]][travis-url]
[![Coverage Status][coveralls-image]][coveralls-url]

[travis-image]: https://travis-ci.org/jackhutu/jackblog-api-express.svg?branch=master
[travis-url]: https://travis-ci.org/jackhutu/jackblog-api-express

[coveralls-image]: https://coveralls.io/repos/jackhutu/jackblog-api-express/badge.svg?branch=master&service=github
[coveralls-url]: https://coveralls.io/github/jackhutu/jackblog-api-express?branch=master

## 简介
Jackblog 是使用 Node.js + MongoDB + 其它客户端框架, 开发的个人博客系统,前后端分离,仿简书模板.此为服务端express版.   
服务端有:  
[express版](https://github.com/jackhutu/jackblog-api-express)  
[koa版](https://github.com/jackhutu/jackblog-api-koa)         
客户端有:  
[angular1.x版](https://github.com/jackhutu/jackblog-angular1)   
[react redux 版](https://github.com/jackhutu/jackblog-react-redux)  
[vue 版](https://github.com/jackhutu/jackblog-vue)    
移动端有:   
[react native 版](https://github.com/jackhutu/jackblog-react-native-redux)

## 环境准备
```
node.js 4.0+
mognodb 3.0+
```

## 配置
* 配置文件路径: ./server/config/env, 可将私有配置放入./server/config/env/private 下.
* [七牛云存储配置](https://portal.qiniu.com/signup?code=3lg7fovhjx2ky)  

```
  qiniu:{
    app_key:"app_key",
    app_secret:"app_secret",
    domain:"domain",          //七牛配置域名
    bucket:"bucket"           //七牛空间名称  
  },
```

## 开发
```
$ npm install
$ gulp serve
```
配合客户端测试的测试模式   
 
```
$ gulp serve:test
```

## 线上布署
```
$ pm2 start process.json
```
可参考[利用git和pm2一键布署项目到vps](http://angular1.jackhu.top/article/55cd8e00c6e998b817a930c7)

## 测试
```
$ gulp test
```

## License
MIT