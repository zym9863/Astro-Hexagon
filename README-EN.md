English | [简体中文](./README.md)

# Astro Hexagon

A visualization interactive experiment based on Astro: simulating a bouncing ball affected by gravity within a rotating hexagon. This project demonstrates how to combine Canvas, physics simulation, and multi-platform interactive events in Astro.

## ✨ Features

- Real-time rendering of rotating hexagon boundaries, showcasing basic vector graphics.
- Ball physics with gravity, friction, and bounce damping for natural and smooth motion.
- Support for mouse and touch drag interactions to adjust ball position and trajectory.
- Responsive canvas size that automatically recalculates hexagon center and radius on window resize.

## 🎮 Interactions

- Move your mouse or finger over the ball and press down to drag it.
- Release to let the ball continue moving based on its current velocity and direction, colliding with hexagon boundaries.
- Full touch device support with the same interaction as desktop.

## 🚀 Quick Start

Requirements: Node.js ≥ 18, pnpm 8 recommended.

```sh
pnpm install
pnpm dev
```

Development server runs at `http://localhost:4321` by default.

## 📁 Project Structure

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

Core logic is centralized in `src/components/BouncingBall.astro`, handling Canvas rendering, physics simulation, and event listeners.

## 🧞 Common Commands

| Command | Description |
| :--- | :--- |
| `pnpm install` | Install project dependencies |
| `pnpm dev` | Start development server |
| `pnpm build` | Build static site for production to `dist/` |
| `pnpm preview` | Preview build result with local static server |
| `pnpm astro ...` | Run Astro CLI, e.g., `pnpm astro check` |

## 📚 References

- [Astro Documentation](https://docs.astro.build)
- [HTML Canvas API](https://developer.mozilla.org/docs/Web/API/Canvas_API)

Feel free to experiment or extend this project. Submit an Issue or reach out if you have questions.
