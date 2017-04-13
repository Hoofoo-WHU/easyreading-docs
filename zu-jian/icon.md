负责人：王硕

##Icon
变色`SVG`图标解决方案。



###基本用法
- 推荐使用[IconFont](http://www.iconfont.cn)下载的图标
- `SVG`文件中的图形不设置`stroke-width`属性或者设置为`0`
- `SVG`文件中需要在`CSS`中修改颜色的图形不设置`fill`属性
- 将需要使用的svg文件放在`@/components/Icon/svg/`路径中

```html
<icon name="settings" class="icon"></icon>
<!--name属性是SVG文件的文件名-->
```

```js
import Icon from '@/components/Icon'
export default {
    components: {
        Icon
    }
}
```

```css
.icon {
    /*宽高必须设置，否则是0*/
    width: 25px 
    height: 25px
    /*没填颜色的部分默认是黑色，想要透明将颜色设为'#00000000'*/
    color: red
}
```
### Attributes

|参数|说明|类型|可选值|默认值|
|:-----|:-----|:-----|:-----|:-----|
|name|图标的名称|String|`@/components/Icon/svg/`中的`SVG`文件名|-|
|spin|开启旋转动画|Boolean|

