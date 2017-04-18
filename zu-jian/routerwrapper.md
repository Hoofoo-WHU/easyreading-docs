## RouterWrapper
解决`vue-router`的`transition`在`flex`布局下的问题

### 基本使用
```html
<router-wrapper style="flex: 1">
  <transition name="fade">
    <router-view></router-view>
  <transition>
</router-wrapper>
```

```js
import RouterWrapper from '@/components/RouterWrapper'
export default {
  conponents: {
    RouterWrapper
  }
}
```
```css
.slide-fade-enter-active, .slide-fade-leave-active {
  transition: all .8s;
}
.slide-fade-enter, .slide-fade-leave-active {
  opacity: 0;
}
```