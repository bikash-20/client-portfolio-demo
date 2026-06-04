# Core-Engine Portfolio Architecture & Fluid UI Visualizer

An advanced, production-grade portfolio UI built natively with HTML5, pure CSS3, and modern ECMAScript. The design focuses on browser rendering behavior, mouse-parallax tracking, passive scroll handling, and lightweight component lifecycle management without third-party UI frameworks.

## Architectural Intent

The project avoids React, Vue, and similar abstraction layers. It works directly with the DOM lifecycle and critical rendering path so interaction remains lightweight, responsive, and easy to inspect.

## Technical Highlights

- Mouse-parallax orbs driven by normalized viewport coordinates
- Passive scroll listeners to keep scrolling smooth
- Transform-only animation paths to avoid unnecessary layout work
- Dynamic project modal hydration using `dataset` values
- Memory-safe overlay teardown and scroll-state cleanup
- Tokenized color variables for consistent visual styling
- Subtle noise texture and gradient layers for depth

## File Architecture

- `index.html` - semantic structure and page sections
- `styles.css` - token system, layout, responsive rules, and motion styling
- `script.js` - cursor physics, parallax, modal lifecycle, reveal animation, and progress tracking
- `package.json` - minimal project metadata and local preview command
- `package-lock.json` - locked npm metadata for repository scaffolding
- `.gitignore` - standard local development ignores

## Roadmap

- Move inline logic to a Vite build pipeline
- Replace global scroll checks with `IntersectionObserver` pools
- Add lerp-based orbital motion for smoother background motion

## Summary

This portfolio was built independently to explore browser mechanics, math-driven motion, and production-minded frontend structure. It demonstrates self-directed work, performance awareness, and a clean approach to modern web UI engineering.
