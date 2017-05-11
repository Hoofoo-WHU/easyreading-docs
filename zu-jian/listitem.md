负责人：王硕
## ListItem
列表项目，适用于菜单等列表页面

### 基本用法
```html
<template>
<list-item v-for="item in 20" :text="'第'+item+'章'" @tap="tap" style="height: 53px;line-height: 53px;"></list-item>
</template>
```