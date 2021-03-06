# Checkbox 复选框

### 使用指南

在 page.json 中引入组件

```json
"usingComponents": {
  "w-checkbox": "path/to/w-checkbox/index",
}
```

### 代码演示

```html
<w-pane title="Checkbox" desc="复选框" />

<w-pane desc="Default" />
<w-cell-group>
	<w-checkbox options="{{ items1 }}" bind:onChange="handleChange" />
</w-cell-group>

<view>{{ items1Str }}</view>

<w-pane desc="Disabled" />
<w-cell-group>
	<w-checkbox options="{{ items2 }}" bind:onChange="handleChange" />
</w-cell-group>

<w-pane desc="Directon" />
<w-cell-group>
	<w-checkbox
	 direction="right"
	 options="{{ items1 }}"
	 bind:onChange="handleChange"
	/>
</w-cell-group>
```

### API

#### 属性

| 属性      |            说明            |  类型   | 默认值 |
| --------- | :------------------------: | :-----: | -----: |
| color     |            颜色            | string  |      - |
| disabled  |            禁用            | boolean |  false |
| title     |            标题            | string  |      - |
| direction | 方向，可选值有[left/right] | string  |      - |
| options   |                            |  array  |     [] |

#### 事件

| 事件名 | 说明 | 参数 |
| ------ | ---- | ---- |


#### slot

| 名称 | 说明 |
| ---- | ---- |


#### 自定义类名

| 类名       | 说明         |
| ---------- | ------------ |
| wuss-class | 根节点样式类 |
