负责人：王硕

## NavigationBar
顶栏模块，默认`z-index:100`

### 基本用法

- `NavigationBar`作为容器与`NavigationBarItem`成对使用

```html
<navigation-bar :title="title">
  <navigation-bar-item slot="left" text="返回" icon="back" disable/>
  <navigation-bar-item @tap="tap" slot="right" icon="search"  right-icon/>
</navigation-bar>
```
```js
import { NavigationBar, NavigationBarItem } from '@/components/NavigationBar'
export default {
  components: {
    NavigationBar,
    NavigationBarItem
  },
  data () {
    return {
      title: '我是标题党'
    }
  },
  methods: {
    tap () {
      console.log('tap!')
    }
  }
}
```
### NavigationBar Attributes

|参数|说明|类型|可选值|默认值|
|:-----|:-----|:-----|:-----|:-----|
|title|标题文字|`String`|-|`''`|
|sub-title|副标题文字|`String`|-|`''`|

### NavigationBar Slots

|name|说明|
|:-----|:-----|
|-|容纳自定义的顶栏布局，设置后其他`slot`、`title`和`sub-title`失效|
|left|左侧的`NavigationBarItem`|
|right|右侧的`NavigationBarItem`|

### NavigationBarItem Attributes

|参数|说明|类型|可选值|默认值|
|:-----|:-----|:-----|:-----|:-----|
|text|显示的文字|`String`|-|`''`|
|icon|图标的名称|`String`|`@/components/Icon/svg/`中的`SVG`文件名|-|
|right-icon|设置图标位置在右边|`Boolean`|`true`、`false`|`false`|
|disable|设为不可用|`Boolean`|`true`、`false`|`false`|

### NavigationBarItem Events

|事件名称|说明|回调参数|
|:-----|:-----|:-----|
|tap|当用户点击了Item时触发|-|


