负责人：陈一丹

# Modal

模态框

### 基本用法

```html
<template>
    <!--购买框-->
    <modal v-model="shopModalShow" :on-ok="confirmShop" :ok-text="'确认支付'">
        <div slot="header">
            购买本书
        </div>
        <div class="shop-modal">
            <p class="title">{{ shopBook.name }}</p>
            <p class="price">价格：<span>{{ shopBook.price }}</span>代币</p>
            <p class="hold">您还剩余 <span>{{ userHold }}</span>阅币</p>
        </div>
    </modal>
    <!--购买框结束-->
</template>
```

```js
import Modal from '@/components/Modal'
export default {
  components: {
    Modal
  },
  data () {
    return {
      shopModalShow: false
    }
  }
}
```

### Attributes

| 参数 | 说明 | 类型 | 可选 | 默认 |
| :--- | :--- | :--- | :--- | :--- |
| title | 模态框标题 | String |  |  |
| content | 模态框主体内容 | String |  |  |
| showHeader | 是否显示头部 | Boolean | true, false |  |
| showFooter | 是否显示底部 | Boolean | true, false |  |
| showCloseButton | 是否显示关闭按钮 | Boolean | true, false |  |
| showOkButton | 是否显示确认按钮 | Boolean | true, false |  |
| showCancelButton | 是否显示取消按钮 | Boolean | true, false |  |
| okText | 确认按钮上的文字 | String |  | 确认 |
| cancelText | 取消按钮上的文字 | String |  | 取消 |
| onOk | 点击确认按钮绑定的事件 | Function |  |  |
| onCancel | 点击取消按钮绑定的事件 | Function |  |  |

* 使用`v-model`将控制message的展示的参数与组件绑定

### Slots

| name | 说明 |
| :--- | :--- |
| header | 模态框头部 |
| footer | 模态框底部 |
| - | 模态框主体 |



