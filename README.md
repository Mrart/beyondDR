# beyondDR
## 目录结构
```
├── cfg                     # webpack和npm运行的脚本配置
├── dist                    # 编译之后代码位置
├── karma.conf.js           # karma测试的配置文件
├── node_modules            # 第三方依赖和工具存放位置
├── package.json            # npm配置文件
├── server.js               # webpack-dev-server启动
├── src                     # 源代码文件
│   ├── actions             # redux的action文件
│   ├── components          # react的组件
│   ├── config              # 不同环境下的配置文件
│   ├── images              # 图片文件
│   ├── reducers            # redux的reduce文件
│   ├── stores              # redux的store文件
│   ├── styles              # 样式文件
│   ├── index.html          
│   └── index.js
├── test                    # 测试文件
│   ├── actions
│   ├── components
│   ├── config
│   ├── helpers
│   ├── loadtests.js
│   ├── sources
│   └── stores
└── webpack.config.js       # webpack配置文件
```

## 使用方法
1. 获得最新版本到本地
```
$ git clone https://github.com/DashShen/beyondDR.git
```


2. 执行npm install 命令下载依赖包
```
$ npm install
```

3. 执行npm start 启动
```
$ npm start
```
> 执行该命令会在浏览器中打开地址为[localhost:8000/webpack-dev-server/](http://localhost:8000/webpack-dev-server/)的窗口用于开发调试,不会在dist目录下生产代码，并且相应的代码修改会进行热加载

## Build, Test
- 如果希望在dist目录下生成代码文件，执行
```
$ npm run dist
```
> 执行完命令之后，会在dist目录下生成此版本的可部署代码

- 如果想进行代码的语法与风格检查,执行
```
$ npm run lint
```

- 如果想使用karma进行测试,执行下列命令
```
$ npm run test
```






