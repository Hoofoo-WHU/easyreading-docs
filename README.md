## 技术栈

- [Vue.js](https://cn.vuejs.org/v2/guide/)
- [Vuex](https://vuex.vuejs.org/zh-cn/)
- [vue-router](https://router.vuejs.org/zh-cn/)
- [cordova](http://cordova.apache.org/docs/en/latest/)

## 约定

#### 项目结构
```js
easyreading
├── platforms //cordova平台目录，目前包括iOS、Android
├── plugins //cordova插件目录
├── www //cordova挂载目录
├── project //vue.js工程目录
│   ├── build
│   ├── config
│   ├── src //开发目录
│   │   ├── components //组件目录
│   │   ├── modules //模块目录
│   │   ├── router //路由目录
│   │   ├── store //vuex目录
│   │   ├── App.vue //根组件
│   │   ├── main.js //build挂载点
│   │   └── main_dev.js //开发调试挂载点
│   ├── static //全局静态资源
│   └── index.html
└─config.xml //cordova配置文件
```

#### 文档
