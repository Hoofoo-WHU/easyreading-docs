负责人：王硕

## ButtonItem
更接近原生体验的按钮，提供长按触发、滚动失去焦点、滑出取消

### 基本用法

```html
<template>
    <button-item @tap="tap" class="button">{{text}</button-item>
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