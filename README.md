# vditor-theme

vditor适配样式开发

样式参考 [demo](https://goer.icu/vditor-theme)

## 目录结构

```text
├─editor        # 编辑器样式
└─renderer      # 渲染页面样式
```

## 支持的样式

| 样式名 |
| vscode-dark |
| dracula |

## 使用方法

> 参考 [index.html](./docs/vscode-dark.html)

以`vscode-dark`为例

- 全局引入主题

在head标签插入

```html
<link
    rel="stylesheet"
    href="https://cdn.jsdelivr.net/gh/HerbertHe/vditor-theme@main/editor/vscode-dark.css"
/>
```

- 引入内容主题

修改`options.preview`参数

```js
preview: {
    theme: {
        current: "vscode-dark",
        path:
            "https://cdn.jsdelivr.net/gh/HerbertHe/vditor-theme@main/content-theme",
    },
    hljs: {
        style: "solarized-dark256",
    },
},
```
