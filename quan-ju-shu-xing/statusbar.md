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
$statusBar是`cordova-plugin-statusbar`插件的实例，更多使用方法查看[cordova-plugin-statusbar文档](https://github.com/apache/cordova-plugin-statusbar)