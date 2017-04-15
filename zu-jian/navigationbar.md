负责人：王硕

## NavigationBar
顶栏模块

### 基本用法

- `NavigationBar`作为容器与`NavigationBarItem`成对使用

```html
<navigation-bar :title="title">
  <navigation-bar-item slot="left" text="返回" icon="back" disable/>
  <navigation-bar-item slot="right" icon="search"  right-icon/>
</navigation-bar>
```
```js
import { NavigationBar, NavigationBarItem } from '@/components/NavigationBar'
export default {
  components: {
    NavigationBar,
    NavigationBarItem
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

