# prototype-index.html 导入 Figma 说明

## 📋 文件说明

`prototype-index.html` 是一个展示所有界面的主页面，使用 iframe 嵌入各个界面。

## ⚠️ 注意事项

1. **iframe 限制**：Figma 的 HTML 导入插件可能无法解析 iframe 内容
2. **外部依赖**：文件依赖 Tailwind CSS 和 Font Awesome CDN，可能导致显示为黑色
3. **容器页面**：这个文件主要是展示容器，实际内容在 iframe 中

## 🎯 推荐方案

### 方案1：截图导入（最推荐）⭐

**优点**：
- ✅ 完全可靠
- ✅ 可以看到所有界面
- ✅ 不需要处理 iframe 问题

**步骤**：
1. 启动服务器：双击 `start-server.bat`
2. 在浏览器中打开：`http://127.0.0.1:8000/prototype-index.html`
3. 调整浏览器窗口，确保所有界面都可见
4. 使用截图工具截取整个页面
5. 在 Figma 中粘贴（Ctrl+V）
6. 作为参考层使用

### 方案2：分别导入各个界面

**优点**：
- ✅ 每个界面都是独立的，可以单独编辑
- ✅ 转换质量最好

**步骤**：
1. 在 Figma 中安装 `html.to.design` 插件
2. 分别导入以下文件：
   - `home.html`
   - `device-light.html`
   - `device-air.html`
   - `device-temp.html`
   - `devices.html`
   - `rooms.html`
   - `scenes.html`
   - `shop.html`
   - `profile.html`
   - `outdoor.html`

### 方案3：尝试直接导入（可能不工作）

**步骤**：
1. 在 Figma 中安装 `html.to.design` 插件
2. 选择 "Import from File"
3. 选择 `prototype-index.html`
4. **注意**：iframe 内容可能无法显示，只会显示容器框架

## 💡 建议

**最佳工作流程**：
1. 使用方案1（截图）作为整体布局参考
2. 使用方案2（分别导入）来获得可编辑的界面元素
3. 在 Figma 中手动重新组织布局

## 🔧 如果直接导入失败

如果直接导入 `prototype-index.html` 后：
- 显示为黑色 → 这是外部 CDN 无法加载的问题
- iframe 内容为空 → 这是插件无法解析 iframe 的限制

**解决方案**：使用方案1（截图）或方案2（分别导入）

