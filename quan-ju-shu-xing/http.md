负责人：王硕

## $http
实现异步请求

### 基础用法

```javascript
export default {
  methods: {
    logup () {
      this.$http.post('/user/identifier/check', {'identifier': this.phonenum, 'function': 0})
      .then(response => {
        console.log(response.data)
      })
      .catch(error => {
        console.error(error)
      })
    }
  }
}
```
### 说明
$http是Axios的实例，更多详细使用查看[Axios官方文档](https://github.com/mzabriskie/axios)