负责人：陈一丹

# Message

一个简单的消息弹出框

### 基本用法

```html
<template>
    <message v-model="messageShow" :message-text="'购买成功'"></message>
</template>
```

```js
import Message from '@/components/Message'
export default {
  components: {
    Message
  },
  data () {
    return {
      messageShow: false
    }
  }
}
```

### Attributes

| 参数 | 说明 | 类型 | 可选值 | 默认值 |
| :--- | :--- | :--- | :--- | :--- |
| iconName | 图标名称 | String |  | 'ok' |
| messageText | 消息内容 | String |  |  |
| closeTime | 自动消失的时间 | Number |  | 1000 |

* 使用`v-model`将控制message的展示的参数与组件绑定



