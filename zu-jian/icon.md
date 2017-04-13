负责人：王硕

##Icon
变色`SVG`图标解决方案。



###基本用法
- 推荐使用[IconFont](http://www.iconfont.cn)下载的图标
- `SVG`文件中的图形不设置`stroke-width`属性或者设置为`0`
- `SVG`文件中需要在css中修改颜色的图形不设置`fill`属性
- 将需要使用的svg文件放在`@/components/Icon/svg/`路径中

```html
<icon name="settings"></icon>
<!--name属性是SVG文件的文件名-->
```

```
nn
```