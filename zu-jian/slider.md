负责人：陈一丹

# Slider

基于vue-touch的移动端轮播组件

### 基本用法

```html
<template>
    <slider :imgUrl="urlArr" :changeSpeed="3000" @tap="tapAction"></slider>
</template>
```

```js
import Slider from '@/components/Slider'
export default {
  components: {
    Slider
  },
  data () {
    return {
      urlArr: [
        {id: 1, url: 'xxxx'},
        {id: 2, url: 'xxxx'},
        {id: 3, url: 'xxxx'}
      ]
    }
  },
  methods: {
    tapAction (id) {
      console.log('id')
    }
  }
}
```

* `imgUrl`需要遵循数据格式，这是一个对象数组，对象里有图片id和图片url两个属性，id可以理解为图片展示的顺序
* 绑定的`tap`\(点击\)事件，会返回一个图片id，可根据id判断点击的是哪一张图片，从而进行事件处理

### Attributes

| 参数 | 说明 | 类型 | 可选值 | 默认值 |
| :--- | :--- | :--- | :--- | :--- |
| imgUrl | 图片的url | Arrary |  | 默认含有来源网络的三张图片 |
| changeSpeed | 图片自动播放的速度 | Number |  | 3000/ms |

### Events

| 事件名称 | 说明 | 参数 |
| :--- | :--- | :--- |
| tap | 点击事件 | id（由组件传递出来） |



