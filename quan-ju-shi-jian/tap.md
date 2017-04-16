负责人：王硕
## Tap
替代`Click`事件，迅速响应触摸事件

### 说明
随阅易项目中，对于所有未给出触摸事件的组件的`Click`事件全部需要由`v-tap`指令来实现，`v-tap`指令来源于 [Vue-Tap插件](https://github.com/MeCKodo/vue-tap)，用于快速相应用户的触摸事件。

### 基本用法

```html
<ul>
  <li v-for="(item,index) in list" v-tap="{ methods:args , index : index, item:item }">
		{{item.name}}---{{item.age}}
  </li>
</ul>
```

```javascript
methods : {
  args : function(params) {
    // v-for循环带参数的回调
    console.log('---params.event---',params.event) // 原生事件
    console.log('---params.tapObj---',params.tapObj)
    console.log('---params.index---',params.index)
    console.log('---params.el---',params.el)
    //params.tapObj 可获得 tap的一些参数
    //pageX,pageY,clientX,clientY,distanceX,distanceY
    //后面2个分别的手指可能移动的位置(以后可用于拓展手势)
  }
}
```