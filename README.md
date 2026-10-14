# 《百年孤独》布恩迪亚家族谱

由 Albert King 制作。保留原 Site 的 HTML、CSS、JavaScript 与人物图片，支持桌面与手机。

## 结构

- `dist/index.html`：页面
- `dist/style.css`：视觉及响应式样式
- `dist/data.js`：人物资料
- `dist/app.js`：族谱、搜索、代际阅读、详情与关系交互
- `dist/assets/`：人物肖像与马孔多背景

## 发布

将 GitHub Pages 的 Source 设置为 GitHub Actions。推送到 `main` 后，工作流检查 JavaScript 并打包 `dist/`，自动部署至 Pages。本站无需编译步骤或外部后端。

## 自然语言维护

在可访问此仓库的 ChatGPT / Codex 中描述修改需求，预览并确认后，由代理提交和推送。仓库授权与写入能力须在当前会话中有效。GitHub Actions 负责提交之后的部署，不负责自动获取其他 ChatGPT Site 的更改。

## 回退

对需要撤销的提交执行 `git revert <提交号>` 并推送；部署工作流自动发布回退后的版本。本仓库从最终确认版本开始记录历史，不迁入原 Site 的过程版本。
