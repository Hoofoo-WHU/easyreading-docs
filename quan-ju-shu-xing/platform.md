负责人：王硕

## $platform
判断运行平台

### 基础用法

```js
export default {
  computed: {
    ios: function () {
      return this.$platform === 'ios' //运行平台为ios
    },
    android: function () {
      return this.$platform === 'android' //运行平台为android
    },
    dev: function () {
      return this.$platform === 'dev' //运行平台为开发平台
    }
  }
}
```

### 可选值
|iOS|Android|Development|
|:------|:------|:------|
|`ios`|`android`|`dev`|