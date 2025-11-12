# React JavaScript Demo

一个基于 [Create React App](https://create-react-app.dev/) 的 React JavaScript 应用示例项目。使用纯 JavaScript（无 TypeScript）构建 React 单页应用。

## 技术栈

- **React**: 19.2.0
- **React Scripts**: 5.0.1
- **Testing Library**: 完整的测试工具链
- **Web Vitals**: 性能监控

## 项目结构

```
react-js-demo/
├── src/
│   ├── App.js             # 主应用组件
│   ├── index.js           # 应用入口
│   ├── index.css          # 全局样式
│   └── components/        # React 组件
├── public/                # 静态资源
│   ├── index.html
│   └── ...
├── package.json           # 项目依赖配置
└── README.md
```

## 功能特性

- React 19 支持
- 纯 JavaScript（无 TypeScript）
- 完整的测试工具链
- Web Vitals 性能监控
- 热重载开发体验
- 生产就绪的构建配置

## 快速开始

### 前置要求

- Node.js 14 或更高版本
- npm 或 yarn

### 安装和运行

```bash
# 克隆项目
git clone <repository-url>
cd react-js-demo

# 安装依赖
npm install
# 或
yarn install

# 运行开发服务器
npm start
# 或
yarn start
```

应用将在 `http://localhost:3000` 启动。

### 构建和测试

```bash
# 构建生产版本
npm run build

# 运行测试
npm test

# 弹出配置（不推荐，除非必要）
npm run eject
```

## 项目特点

### Create React App

使用 Create React App (CRA) 作为基础：
- 零配置设置
- 开箱即用的工具链
- Webpack 配置已优化
- 生产就绪的构建

### 纯 JavaScript

项目使用纯 JavaScript，无需类型定义：
- 更快的开发速度
- 更少的配置
- 适合快速原型开发
- 易于学习和理解

### React 19

使用最新的 React 19 特性：
- 改进的并发渲染
- 新的 Hooks
- 更好的性能

## 开发

### 热重载

CRA 提供快速刷新功能，修改代码会自动更新。

### 环境变量

支持环境变量配置：

```bash
# .env
REACT_APP_API_URL=https://api.example.com
```

### 代理配置

可以在 `package.json` 中配置代理：

```json
{
  "proxy": "http://localhost:4000"
}
```

## 测试

### 运行测试

```bash
npm test
```

使用 Jest 和 React Testing Library：
- 单元测试
- 集成测试
- 快照测试
- 覆盖率报告

### 测试示例

```javascript
import { render, screen } from '@testing-library/react';
import App from './App';

test('renders learn react link', () => {
  render(<App />);
  const linkElement = screen.getByText(/learn react/i);
  expect(linkElement).toBeInTheDocument();
});
```

## 构建和部署

### 生产构建

```bash
npm run build
```

构建输出在 `build` 目录，包含：
- 优化的 JavaScript 和 CSS
- 代码分割
- 资源优化
- 源映射

### 部署选项

- **Netlify**: 自动部署
- **Vercel**: 零配置部署
- **GitHub Pages**: 静态托管
- **AWS S3 + CloudFront**: 企业级部署

## 性能优化

### Web Vitals

项目集成了 Web Vitals 监控：
- Core Web Vitals 指标
- 性能报告
- 用户体验指标

### 代码分割

CRA 自动进行代码分割：
- 路由级别的分割
- 动态导入支持
- 懒加载组件

## 与 TypeScript 版本的区别

- **无类型检查**: JavaScript 版本没有编译时类型检查
- **更快的开发**: 无需等待 TypeScript 编译
- **更灵活**: 可以更快速地迭代和实验
- **适合原型**: 适合快速原型开发和学习

## 参考资源

- [Create React App 文档](https://create-react-app.dev/)
- [React 文档](https://react.dev/)
- [React Testing Library](https://testing-library.com/react)
- [Web Vitals](https://web.dev/vitals/)
