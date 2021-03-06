# Steps 步骤条

### 使用指南

在 page.json 中引入组件

```json
"usingComponents": {
  "w-steps": "path/to/w-steps/index",
}
```

### 代码演示

```html
<w-pane title="Steps" desc="步骤条" />

<w-pane desc="Default" />
<w-steps
bindcomplete="complete"
current="{{ current }}"
steps="{{ steps }}"
/>

<w-button bind:click="setCurrent" size="small" type="info">下一步</w-button>
<w-pane desc="vertical" />
<w-steps
current="{{ current }}"
steps="{{ steps }}"
direction="vertical"
/>

<w-pane desc="error" />
<w-steps current="2" steps="{{ steps2 }}" />
<w-pane desc="dot" />
<w-steps current="2" type="dot" steps="{{ steps2 }}" />
```

### API

#### 属性

| 属性      |                说明                |  类型  |    默认值 |
| --------- | :--------------------------------: | :----: | --------: |
| steps     |              步骤数组              | array  |         - |
| type      |    类型数组型 number 点状型 dot    | string |         - |
| direction | 横向和竖向'vertical'\|'horizontal' | string |         - |
| current   |   指定当前步骤，从 0 开始记数。    | number | undefined |

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
