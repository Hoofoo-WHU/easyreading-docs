负责人：王硕

## $statusBar
控制手机状态栏

### 基础用法

```javascript
export default {
  methods: {
    show () {
      if (this.$statusBar) {
        this.$statusBar.show()
      }
    },
    hide () {
      if (this.$statusBar) {
        this.$statusBar.hide()
      }
    }
  }
}
```
### 说明
$http是Axios的实例，更多详细使用查看[Axios官方文档](https://github.com/mzabriskie/axios)