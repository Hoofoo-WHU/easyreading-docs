负责人：王硕
## Touch
移动端触屏事件的解决方案

### 说明
随阅易项目中，对于所有未给出触摸事件的组件c，所有的触摸事件都由`touch`来实现，`touch`来源于[vue-touch](https://github.com/vuejs/vue-touch/tree/next)插件，基于`Hammer.js`，这里只介绍基本的使用方法，详情请查看[vue-touch文档](https://github.com/vuejs/vue-touch/tree/next)。

### 基本使用
```html
<touch @tap="tap">
  <div class="content"></div>
</touch>
<!--touch标签相当于一个div-->
```
```js
export default {
  methods: {
    tap () {
      console.log('tap!')
    }
  }
}
```
### 支持的操作
`pan`、`pinch`、`rotate`、`swipe`、`tap`，详情请查看[vue-touch文档](https://github.com/vuejs/vue-touch/tree/next)。

