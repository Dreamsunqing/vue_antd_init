# 更新日志

## 2023-10-27

- 清理了 Vue 项目的默认样式和组件。
  - 移除了 `App.vue` 中的默认内容和样式。
  - 删除了 `src/components/HelloWorld.vue`、`src/components/TheWelcome.vue` 和 `src/components/WelcomeItem.vue`。
  - 确认 `main.ts` 已正确引入 Ant Design Vue。
- 更新了 Vue Router 配置。
  - 删除了 `src/views/HomeView.vue` 和 `src/views/AboutView.vue` 默认视图文件。
  - 移除了 `src/router/index.ts` 中指向这些默认视图的路由配置。
- 移除了 `src/assets` 文件夹中的默认样式文件（`main.css` 和 `base.css`）。
- 重新添加并引入了默认路由 `HomeView`。
  - 在 `src/views` 目录下创建了 `HomeView.vue` 文件。
  - 更新了 `src/router/index.ts`，添加了 `/` 路径指向 `HomeView`。
- 创建了 `.gitignore` 文件，并添加了常见的 Vue/Vite 项目忽略规则。

## 2024-05-24

- 安装了 Ant Design Vue 依赖。
- 在 `src/components` 目录下创建了以下布局组件：
  - `PageHeader.vue` (头部组件)
  - `PageSider.vue` (侧边栏组件)
  - `PageContent.vue` (内容区域组件)
  - `PageFooter.vue` (底部组件)
- 修改了 `src/App.vue` 文件，使用 Ant Design 的 `Layout` 组件构建了整体布局，并引入了上述模块化组件。
- 更新了 `README.md` 文件，详细描述了 Ant Design 布局结构、页面用途和样式说明。
- 修复了 `PageHeader.vue` 中导航部分的白色背景问题，将 `a-layout-header` 的背景色修改为深色，并调整了 `.logo` 的背景色。
- 修复了 `PageHeader.vue` 中 `logo` 部分的深灰色矩形框问题，移除了 `.logo` 的背景色，使其透明。
