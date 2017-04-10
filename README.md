## 技术栈
随阅易前端项目开发将涉及但不限于以下技术：
[`Vue.js`](https://cn.vuejs.org/v2/guide/) [`Vuex`](https://vuex.vuejs.org/zh-cn/) [`vue-router`](https://router.vuejs.org/zh-cn/) [`cordova`](http://cordova.apache.org/docs/en/latest/)

## 约定
由于随阅易前端项目是一个多人合作项目，所以需要一些所有人需要遵守的约定来保证项目可以稳定的进行开发。
### GitHub
随阅易前端项目托管于`GitHub`，包括`master`、`dev`以及以每位开发人员名字命名的分支，为了避免不必要的冲突，开发人员仅能通过以自己名字命名的分支，再通过`pull request`请求合并。
> **[danger] 警告**
>
> 遇到问题可以查看文档或与相关开发人员联系，**一定**不要修改他人负责的代码！

### 目录结构
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
> **[info] 提示**
>
> 项目中的 **components** 和 **modules** 目录都是存放 **.vue** 文件，前者存放会被重用的基础组件，后者存放搭建框架的基础模块。

### 编写文档
随阅易前端项目文档采用`markdown`编写，每个Vue组件都应该编写以相应名称命名的文档，如果组件涉及以下内容，则**必须**书写清楚。

#### 作者
对应Vue组件的作者，为了能及时沟通修改，请**务必**注明组件作者。

#### 介绍
为了其他人的使用，请简要说明组件的作用。

#### 基本用法
说明组件的基本使用方法，有必要的话请给出代码示例。

#### Attributes

对应Vue组件的props，格式如下例所示：

|参数|说明|类型|可选值|默认值|
|:-----|:-----|:-----|:-----|:-----|
|size|控件的大小|string|large、normal、small|-|

#### Events
对应Vue组件会触发的事件，格式如下例所示：

|事件名称|说明|回调参数|
|:-----|:-----|:-----|
|change|绑定值变化时触发的事件|选中的 Radio label 值|

#### Slots
对应Vue组件的分发内容，格式如下例所示：

|name|说明|
|:-----|:-----|
|-|显示的内容|
|title|标题区的内容|

#### Functions
对应Vue组件的方法，只需要注明公开的方法即可，格式如下例所示：

|方法名|说明|
|:-----|:-----|
|open|打开当前实例|
|close|关闭当前实例|





