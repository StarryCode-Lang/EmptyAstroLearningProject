# 项目结构

## 目录组织

```
/
├── public/                 # 静态资源目录
│   └── favicon.svg        # 网站图标
├── src/                   # 源代码目录
│   ├── assets/           # 资源文件 (图片、SVG等)
│   │   ├── astro.svg
│   │   └── background.svg
│   ├── components/       # 可复用组件
│   │   └── Welcome.astro
│   ├── layouts/          # 页面布局组件
│   │   └── Layout.astro
│   └── pages/            # 页面路由 (基于文件的路由)
│       ├── posts/        # 博客文章目录
│       ├── about.astro   # 关于页面
│       ├── blog.astro    # 博客列表页
│       └── index.astro   # 首页
├── .kiro/                # Kiro 配置目录
│   └── steering/         # AI 助手指导规则
├── astro.config.mjs      # Astro 配置文件
├── package.json          # 项目依赖和脚本
└── tsconfig.json         # TypeScript 配置
```

## 文件命名约定
- **页面文件**: 使用 `.astro` 扩展名，放在 `src/pages/` 目录
- **组件文件**: 使用 `.astro` 扩展名，放在 `src/components/` 目录
- **布局文件**: 使用 `.astro` 扩展名，放在 `src/layouts/` 目录
- **静态资源**: 放在 `public/` 目录，可直接通过根路径访问

## 路由规则
- 基于文件系统的路由
- `src/pages/index.astro` → `/` (首页)
- `src/pages/about.astro` → `/about/` (关于页面)
- `src/pages/blog.astro` → `/blog/` (博客页面)
- `src/pages/posts/` → `/posts/` (博客文章目录)

## 组件导入规则
- 使用相对路径导入组件: `import Layout from "../layouts/Layout.astro"`
- 资源文件导入: `import astroLogo from '../assets/astro.svg'`
- 组件应该被实际使用，避免未使用的导入