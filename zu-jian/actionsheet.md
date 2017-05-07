负责人：王硕
## ActionSheet
底部弹出组件，单独使用或配合`ActionSheetItem`进行划分区域使用，默认`z-index:300`。

### 基本用法

```html
<action-sheet :show="show" @cancel="cancel">
  <action-sheet-item>
    <button @click="click('item1')">item1</button>
  </action-sheet-item>
  <action-sheet-item>
    <button @click="click('item2')">item2</button>
  </action-sheet-item>
</action-sheet>
```
```javascript
import { ActionSheet, ActionSheetItem } from '@/components/ActionSheet'
export default {
  components: {
    ActionSheet,
    ActionSheetItem
  },
  data () {
    return {
      show: false
    }
  },
  methods: {
    showActionSheet () {
      this.show = true
    },
    cancel () {
      this.show = false
    },
    click (item) {
      console.log(item)
    }
  }
}

```
### ActionSheet Attributes

|参数|说明|类型|可选值|默认值|
|:-----|:-----|:-----|:-----|:-----|
|show|是否显示|`Boolean`|`true`、`false`|`false`|


### ActionSheet Events

|事件名称|说明|回调参数|
|:-----|:-----|:-----|
|cancel|当用户点击了Cancel时触发|-|

### ActionSheet Slots

|name|说明|
|:-----|:-----|
|-|ActionSheet的内容，可以使用ActionSheetItem进行垂直划分区域|

### ActionSheetItem Slots

|name|说明|
|:-----|:-----|
|-|ActionSheetItem的内容|

