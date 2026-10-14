# 网站维护规则

- 网站是纯静态站点，生产文件在 `dist/`。无需 npm 安装或框架构建。
- 保持现有视觉、内容与交互，除非用户明确要求修改。
- 所有本地资源使用相对路径，兼容 GitHub Pages 的 `/macondo-family-tree/` 子路径。
- 修改后运行 `node --check dist/app.js` 与 `node --check dist/data.js`，检查资源完整性，并在可用的浏览器中验证桌面和手机布局、搜索、代际切换、人物介绍、关系跳转和缩放。
- 先向用户展示修改结果。仅在用户确认该次修改后提交并推送到 GitHub `main`。
- `main` 的推送触发 `.github/workflows/pages.yml` 自动部署；检查 Actions 成功状态后报告发布地址。
- 回退使用 `git revert` 创建新提交，保留历史；不要强制推送或改写历史。
- 不提交任何凭据、令牌、运行时文件或个人配置。
- 以 GitHub 仓库为维护主线；原 ChatGPT Site 的更新不会自动同步到此仓库。
