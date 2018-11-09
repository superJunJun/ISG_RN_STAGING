# ISG_RN_STAGING
## 准备工作
- node.js环境（npm包管理器）

## 开发运行
```bash
   
    # 安装依赖
    npm install
 
    # 本地开发 开启服务
    npm start
    常见问题：1、关闭本地代理

```
浏览器访问 http://localhost:8081

## 目录结构
```shell
├── build                      // 构建相关  
├── config                     // 配置相关
├── ios                        // ios工程源代码
├── android                    // android工程源代码
├── src                        // 源代码
│   ├── api                    // 所有请求
│   ├── assets                 // 主题 字体等静态资源
│   ├── components             // 全局公用组件
│   ├── directive              // 全局指令
│   ├── filtres                // 全局filter
│   ├── mock                   // mock数据
│   ├── router                 // 路由
│   ├── store                  // 全局store管理
│   ├── styles                 // 全局样式
│   ├── utils                  // 全局公用方法
│   ├── view                   // view
│   ├── App.vue                // 入口页面
│   └── main.js                // 入口 加载组件 初始化等
├── static                     // 第三方不打包资源
│   ├── jquery
│   └── Tinymce                // 富文本
├── .babelrc                   // babel-loader 配置
├── eslintrc.js                // eslint 配置项
├── .gitignore                 // git 忽略项
├── favicon.ico                // favicon图标
├── index.js                   // 项目入口
└── package.json               // package.json
├── bundle_cmd.txt             // 打包命令展示
├── common_dependence.js       // 基础包打包依赖
└── jsbundle.business.config.js               // 业务bundle 打包实现函数声明
└── jsbundle.common.config.js                 // 基础bundle 打包实现函数声明

```

## 版本要求
react-native 版本  必须 0.57.0 （爱上岗平台引入react-native版本0.57.0）
react 版本  0.16.5
更多第三方控件及版本使用    参考common_dependence.js 及 package.json

！版本必须严格相同 ！
如有未引用第三方 请联系爱上岗工作人员 邮件地址：lijun@ishanggang.com

## 发布
```bash
    # 发布测试
    1. 参考bundle_cmd.txt 内容 分包打包
    2. 以项目名创建文件（如fbi,保证唯一性）把业务包放入，压缩为zip 上传到爱上岗中控平台

    # 构建生成环境
    npm run build:prod
```

## 感谢
感谢作者：[PanJiaChen](https://github.com/PanJiaChen/vue-element-admin)

## License

Apache License Version 2.0
