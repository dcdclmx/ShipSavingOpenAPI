# 📘 ShipSaving API 文档使用说明（Swagger UI 版本）

## 📊 API 文档格式对比：传统 PDF vs Swagger UI

| 特性 | PDF 文档 | Swagger UI |
|------|-----------|-------------|
| 🖱 交互性 | ❌ 静态文档，仅能查看 | ✅ 支持 Try it out、在线测试接口 |
| 🔄 实时更新 | ❌ 更新不方便，需要重新导出 | ✅ 只需修改 YAML 并推送，即可自动更新页面 |
| 🧩 结构清晰 | ❌ 多为手动排版，查找字段困难 | ✅ 自动按 API 分组，参数/响应一目了然 |
| 📱 开发者友好 | ⚠️ 需人工复制示例或 URL 测试 | ✅ 自动生成 curl、Request body、响应等说明 |
| 🌐 部署方式 | ❌ 需要手动发送文件或放在静态页面 | ✅ 可用 GitHub Pages 自动部署、在线访问 |
| 📎 扩展能力 | ❌ 无法动态链接文档内容 | ✅ 可内嵌外部文档、使用 Markdown 描述、支持 OAuth 等 |

---

## 🚀 Swagger UI 使用流程

### 1. 编辑文档

编辑 `dist/swagger.yaml` 文件，即为 API 主文档。

推荐工具：
- [Swagger Editor](https://editor.swagger.io)
- VS Code + OpenAPI 插件

---

### 2. 提交并部署

```bash
git add dist/swagger.yaml
git commit -m "update API doc"
git push
```

GitHub Pages 会自动展示 `dist/index.html`，页面加载了 `swagger.yaml` 并渲染出 Swagger UI。

访问地址类似于：

```
https://yourusername.github.io/openAPI/
```

---

### 3. 使用和分享

- 页面中可直接查看每个接口的参数、响应、示例
- 点击 **Try it out** 可直接测试接口
- 支持 curl / Fetch / Axios 代码片段查看
- 无需查阅 PDF 或手动发请求


