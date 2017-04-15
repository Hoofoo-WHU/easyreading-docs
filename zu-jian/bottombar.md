负责人：王硕

## BottomBar
底栏模块

### 基本用法

- `BottomBar`作为容器与`BottomBarItem`成对使用

```html
<bottom-bar class="bottom-bar">
  <bottom-bar-item icon="settings" name="设置" :active="active"></bottom-bar-item>
</bottom-bar>
```
```js
import { BottomBar, BottomBarItem } from '@/component/BottomBar'
export default {
  components: {
    BottomBar,
    BottomBarItem
  },
  data () {
    return {
      active: true
    }
  }
}
```

### BottomBar Slots

|name|说明|
|:-----|:-----|
|-|容纳BottomBarItems|

### BottomBarItem Attributes

|参数|说明|类型|可选值|默认值|
|:-----|:-----|:-----|:-----|:-----|
|name|显示的文字|String|-|`bottom-bar-item`|
|icon|图标的名称|String|`@/components/Icon/svg/`中的`SVG`文件名|-|
|active|激活状态|Boolean|`true`、`false`|`false`|
|disable|设为不可用|Boolean|`true`、`false`|`false`|

