## 技术栈
随阅易前端项目开发将涉及但不限于以下技术：
- [Vue.js](https://cn.vuejs.org/v2/guide/)
- [Vuex](https://vuex.vuejs.org/zh-cn/)
- [vue-router](https://router.vuejs.org/zh-cn/)
- [cordova](http://cordova.apache.org/docs/en/latest/)

## 约定
由于随阅易前端项目是一个多人合作项目，所以需要一些所有人需要遵守的约定来保证项目可以稳定的进行开发。
#### GitHub
随阅易前端项目托管于`GitHub`，包括`master`、`dev`以及以每位开发人员名字命名的分支，为了避免不必要的冲突，开发人员仅能通过以自己名字命名的分支，再通过`pull request`请求合并。
> **[danger]警告**
>
> 遇到问题可以查看文档或与相关开发人员联系，**一定**不要修改他人负责的代码！

#### 结构
开发可能涉及到的目录结构如下：
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
│   └── index.html
└─config.xml //cordova配置文件
```

#### 文档
