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
|border|是否显示边框|`Boolean`|-|`加载中...`|


### Events

|事件名称|说明|回调参数|
|:-----|:-----|:-----|
|beforeScrollStart|在用户触摸屏幕但还没有开始滚动时触发|-|
|scrollStart|开始滚动时触发|-|
|scrollEnd|停止滚动时触发|-|
|pullRefresh|下拉刷新时触发|`over`:通知`Scroller`刷新完毕|

### Slots

|name|说明|
|:-----|:-----|
|-|滚动内容|

### Functions

|方法名|说明|参数|
|:-----|:-----|:-----|
|scrollTop|滚动到顶部|-|
|scrollTo|滚动到任意的位置|x:横坐标,y:纵坐标|
|scrollBy|从当前位置进行滚动|x:横坐标,y:纵坐标|
|refresh|刷新滚动区域大小，当滚动内容改动后需要调用|-|









