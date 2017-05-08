负责人：王硕
## Container
用来纵向分割布局的容器，主要用于`Scroller`中

### 基本用法
``` html
<scroller style="flex-grow: 1" ref="scroller">
  <container title="标题1">
    <!--内容1-->
  </container>
  <container title="标题2">
    <!--内容2-->
  </container>
</scroller>
```
```js
import Scroller from '@/components/Scroller'
import Container from '@/components/Container'
export default {
  components: {
    Scroller,
    Container
  }
}

### Container Attributes

|参数|说明|类型|可选值|默认值|
|:-----|:-----|:-----|:-----|:-----|
|title|标题|`String`|-|`""`|
|border|是否显示边框|`Boolean`|`true`、`false`|`true`|


### Slots

|name|说明|
|:-----|:-----|
|-|内容|
|title|自定义标题样式|










