负责人：王硕
## Scroller
跨平台相同操作体验的滚动组件。

### 基本用法
``` html
<scroller style="flex: 1" ref="scroller">
  <div>content</div>
</scroller>
```
```js
import Scroller from '@/components/Scroller'
export default {
  components: {
    Scroller
  },
  methods: {
    scrollTop () {
      this.$refs.scroller.scrollTop()
    }
  }
}
```
> **[danger] 注意**
>
> Scroller一定要设置大小且滚动内容不能脱离文档流，否则将无法正常运行。

### Events

|事件名称|说明|回调参数|
|:-----|:-----|:-----|
|beforeScrollStart|在用户触摸屏幕但还没有开始滚动时触发|-|
|scrollStart|开始滚动时触发|-|
|scrollEnd|停止滚动时触发|-|

### Slots

|name|说明|
|:-----|:-----|
|-|滚动内容|


### Functions
对应Vue组件的方法，只需要注明公开的方法即可，格式如下例所示：

|方法名|说明|参数|
|:-----|:-----|:-----|
|scrollTop|滚动到顶部|-|
|scrollTo|滚动到坐标值|x:横坐标,y:纵坐标|











