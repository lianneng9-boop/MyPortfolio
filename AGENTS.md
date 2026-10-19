
---

### 3. 文件三：`AGENTS.md` （AI 代理指令/开发规范）
**在 VS Code 新建文件 `AGENTS.md`，粘贴以下内容：**

```markdown
# AI 开发规范与指令 (AGENTS)

## 一、项目概述
这是一个个人作品集网站，包含前台展示和后台管理。要求界面简洁现代，深色主题。

## 二、开发规范
1. **代码风格**：使用函数式组件（Functional Components）和 React Hooks。
2. **样式规范**：全部使用 TailwindCSS 编写，禁止写行内样式或外部 CSS 文件（除了 index.css 引入 Tailwind）。
3. **目录约束**：页面组件放在 `src/pages`，复用组件放在 `src/components`。
4. **数据交互**：禁止直接操作 `localStorage`，必须通过 `src/api.js` 统一封装的方法进行读写。

## 三、测试要求
- 每次新增功能后，必须在本地运行 `npm run dev` 确认无报错。
- 测试表单提交功能，确保数据能正确存入 localStorage。

## 四、注意事项
- 后台登录密码暂时写死为 `123456`。
- 移动端适配必须完善，导航栏在小屏幕下需折叠。
- 每次生成代码后，必须保证不报错、能直接运行。