# Known Limitations

- VS Code 的静态编辑器分割线宽度由 Workbench 控制，主题只能改颜色，不能把 `editorGroup.border` 直接加粗。`workbench.sash.size` 只能扩大拖拽热区和 hover 感知，不会把静态线条变成多像素。
- VS Code 的 `editor.lineHighlightBackground` 作用于逻辑行，不是自动换行后的显示行。本项目保留细灰色边框式光标行效果，不再尝试用背景模拟 Overleaf 的显示行高亮。
- 裸 `^`、`_` 的浅红背景依赖语法或诊断系统把文本标成 invalid。主题只能给 invalid token 上色，不能自己判定 LaTeX 是否非法。
- Overleaf 使用 CodeMirror/Lezer 解析和网页 CSS；VS Code 使用 TextMate token 与主题规则。两者语法模型不同，所以无法做到逐字符完全一致。
- 本项目不使用自定义 CSS 注入，因此不能修改 VS Code 没暴露给主题 API 的布局细节。
- 推荐排版命令修改的是用户级 VS Code 设置，不是主题 JSON。这样才能控制字体、字号、行高、自动换行等非主题字段。
