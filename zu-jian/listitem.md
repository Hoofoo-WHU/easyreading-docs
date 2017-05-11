负责人：王硕
## ListItem
列表项目，适用于菜单等列表页面

### 基本用法
```html
<template>
  <list-item v-for="item in 20" :text="'第'+item+'章'" @tap="tap" style="height: 53px;line-height: 53px;"></list-item>
</template>
```
```js
import ListItem from '@/components/ListItem'
export default {
  components: {
    ListItem
  },
  methods: {
    tap () {
      console.log('tap')
    }
  }
}
```
### ActionSheet Attributes

|参数|说明|类型|可选值|默认值|
|:-----|:-----|:-----|:-----|:-----|
|text|显示的文字|`String`|-|`''`|
|icon|左侧图标的名称|`String`|`@/components/Icon/svg/`中的`SVG`文件名|-|
|right|显示默认的右箭头|`Boolean`|`true`、`false`|`false`|


### Slots

|name|说明|
|:-----|:-----|
|-|右侧操作区域（注意事件冒泡）|

### Events

|事件名称|说明|回调参数|
|:-----|:-----|:-----|
|tap|点击操作触发|-|












