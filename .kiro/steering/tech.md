# 技术栈

## 核心框架
- **Astro 5.8.0** - 静态站点生成器，支持组件化开发
- **TypeScript** - 使用严格模式配置 (`astro/tsconfigs/strict`)
- **ES Modules** - 项目使用 ESM 模块系统

## 构建系统
- **包管理器**: npm
- **构建工具**: Astro 内置构建系统
- **配置文件**: `astro.config.mjs` (当前为默认配置)

## 常用命令

| 命令 | 作用 |
|------|------|
| `npm install` | 安装依赖 |
| `npm run dev` | 启动开发服务器 (localhost:4321) |
| `npm run build` | 构建生产版本到 `./dist/` |
| `npm run preview` | 本地预览构建结果 |
| `npm run astro` | 运行 Astro CLI 命令 |

## 开发环境
- **开发服务器**: `localhost:4321`
- **构建输出**: `./dist/` 目录
- **TypeScript**: 启用严格模式检查
- **模块解析**: 支持相对路径导入资源文件