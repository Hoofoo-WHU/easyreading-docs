## RouterContent
配合`RouterWrapper`解决`vue-router`的`transition`在`flex`布局下的问题

### 基本用法
```html
<router-content>
  <div style="flex: 1;" class="content"></div>
</router-content>
```
```js
import RouterContent from '@/components/RouterContent'
export default {
  components: {
    RouterContent
  }
}
```
> **[info]** 提示
**RouterContent**默认使用`flex`布局