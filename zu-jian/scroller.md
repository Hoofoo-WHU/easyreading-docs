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
> Scroller一定要设置大小，否则将无法正常运行。

### Attributes
|参数|说明|类型|可选值|默认值|
|:-----|:-----|:-----|:-----|:-----|
|size|控件的大小|string|large、normal、small|-|


