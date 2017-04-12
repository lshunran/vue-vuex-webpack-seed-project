# vue + vuex + webpack SEED project

> 一个vue + vuex + webpack 的项目脚手架, 来自github上若干个优秀脚手架的整合

## 运行项目

``` bash
# 下载依赖
npm install

# 运行项目
npm run dev

# 打包项目
npm run build

# 打包项目/view the bundle analyzer report
npm run build --report

# 跑单元测试
npm run unit

# 跑e2e测试
npm run e2e

# 统一测试命令
npm test
```

## 项目布局

```
.
├── build                                       // webpack配置文件
├── config                                      // 定义webpack等需要的变量
├── dist                                        // 打包好的静态资源
├── src                                         // 源码目录
│   ├── components                              // 组件
│   │   ├── common                              // 公共组件
│   │   │   └── ...                             // 此处将会放置项目中一些共用的组件
│   │   ├── header                              // 头部公共组件
│   │   │   └── ...                   
│   │   ├── footer                              // 底部公共组件
│   │   │   └── ...                   
│   │   └── ...                                 // 可扩展其他公共组件
│   │       └── ...                       
│   ├── config                                  // 项目基本配置
│   │   ├── routers.js                          // 项目路由配置
│   │   ├── url.js                              // mock测试配置的url
│   │   └── ...                                 // 可扩展一些项目的配置文件
│   ├── assets                                  // 公共静态资源(图片、全局css等)
│   ├── views                                   // 项目页面
│   │   └── index
│   │       ├── index.vue                       // 示例页面
│   │       ├── types.js                        // 定义该页面对应的vuex store中 getters, actions,mutations的静态名称,将在vuex/modules中引入
│   │       └── children                        // 如果该页面有子路由,子路由对应的页面应放置在此文件夹下。注:index为一个页面，index文件夹的结构应和index对应的路由的结构一致!
│   │           ├── child.vue                   // 子路由页面
│   │           └── ..                          // 可扩展
│   ├── plugins                                 // 引用的插件
│   ├── service                                 // 数据交互统一调配
│   │    └── getData.js                         // 获取数据的统一调配文件，对接口进行统一管理。项目统一在此处调用后端的API接口(类似我们angular项目中的service)
│   ├── vuex                                    // vuex的状态管理
│   │    ├── action.js                          // 配置actions
│   │    ├── getters.js                         // 配置getters
│   │    ├── store.js                           // 引用vuex，创建store
│   │    ├── modules                            // store模块
│   │    ├── mutation-types.js                  // 定义常量muations名
│   │    ├── plugins.js                         // 定义vuex plugins
│   │    └── mutations.js                       // 配置mutations
│   │
│   ├── App.vue                                 // 页面入口文件
│   └── main.js                                 // 程序入口文件，加载各种公共组件
├── favicon.ico                                 // 图标
├── index.html                                  // 入口html文件
...
.

```