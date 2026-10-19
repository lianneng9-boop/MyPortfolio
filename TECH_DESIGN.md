# 技术设计文档 (Tech Design)

## 一、技术栈选择
- **前端框架**：React 18 + Vite
- **样式方案**：TailwindCSS
- **路由管理**：React Router DOM
- **状态与数据**：React Hooks (useState, useEffect)

## 二、项目结构
```text
src/
├── api/          # 数据读写层 (使用 localStorage 模拟)
├── components/   # 通用组件 (Navbar, Footer 等)
├── pages/        # 页面组件
│   ├── Home.jsx  # 前台展示页
│   ├── Admin.jsx # 后台管理页 (含登录和表单)
│   └── Blog.jsx  # 博客详情页
├── App.jsx       # 路由配置
└── index.css     # Tailwind 样式引入