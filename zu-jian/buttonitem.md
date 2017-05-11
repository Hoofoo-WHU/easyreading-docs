负责人：王硕

## ButtonItem
更接近原生体验的按钮，提供长按触发、滚动失去焦点、滑出取消，会带来多余的性能消耗，慎用

### 基本用法

```html
<template>
    <button-item @tap="tap" class="button">
    <!-- content -->
    <!-- 默认100%宽度，自动高度，position为relative-->  
    </button-item>
</template>
```
```js
import ButtonItem from '@/components/ButtonItem'
export default {
  name: 'ActionSheetButton',
  components: {
    ButtonItem
  },
  data () {
    return {
    }
  },
  methods: {
    tap () {
      console.log('tap')
    }
  }
}
```
### Slots

|name|说明|
|:-----|:-----|
|-|内容|

### Events

|事件名称|说明|回调参数|
|:-----|:-----|:-----|
|tap|点击操作触发|-|










