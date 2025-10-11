# Astro Hexagon

一个基于 Astro 的可视化交互实验：在旋转的六边形中模拟一颗受重力作用的弹跳小球。项目演示了如何在 Astro 中结合 Canvas、物理模拟与多端交互事件。

## ✨ 功能亮点

- 旋转六边形边界实时绘制，展示基础的矢量图形渲染。
- 小球包含重力、摩擦、反弹阻尼等基础物理规则，表现自然流畅。
- 支持鼠标与触控拖拽，可直接调整小球位置并重新投射。
- 响应式画布尺寸，窗口缩放时自动重新计算六边形中心与半径。

## �️ 交互说明

- 将鼠标或手指移动至小球上按下，即可拖拽移动。
- 松开拖拽后，小球会根据当前速度与方向继续运动并与六边形边界发生碰撞。
- 支持触控设备，操作方式与桌面端一致。

## 🚀 快速开始

环境要求：Node.js ≥ 18，建议使用 pnpm 8。

```sh
pnpm install
pnpm dev
```

默认开发服务器运行在 `http://localhost:4321`。

## 📁 项目结构

```text
Astro-Hexagon/
├── public/
│   └── favicon.svg
├── src/
│   ├── assets/
│   ├── components/
│   │   └── BouncingBall.astro
│   ├── layouts/
│   │   └── Layout.astro
│   └── pages/
│       └── index.astro
├── astro.config.mjs
├── package.json
└── tsconfig.json
```

核心逻辑集中在 `src/components/BouncingBall.astro` 中，负责编写 Canvas 绘制、物理模拟及事件监听。

## 🧞 常用命令

| 命令 | 说明 |
| :--- | :--- |
| `pnpm install` | 安装项目依赖 |
| `pnpm dev` | 启动开发服务器 |
| `pnpm build` | 生成生产环境静态站点至 `dist/` |
| `pnpm preview` | 使用本地静态服务器预览构建结果 |
| `pnpm astro ...` | 运行 Astro CLI，例如 `pnpm astro check` |

## � 参考资源

- [Astro 官方文档](https://docs.astro.build)
- [HTML Canvas API](https://developer.mozilla.org/docs/Web/API/Canvas_API)

欢迎基于本项目进行实验或拓展，若有问题可提交 Issue 或直接交流。
