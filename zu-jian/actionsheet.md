负责人：王硕
## ActionSheet
底部弹出组件，单独使用或配合`ActionSheetItem`进行划分区域使用。

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