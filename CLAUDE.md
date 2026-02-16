# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

A personal portfolio website built with React 19 and Vite. This is a modern single-page application with hot module replacement (HMR) for fast development.

## Development Commands

```bash
# Start development server with HMR (default: http://localhost:5173)
npm run dev

# Build for production (outputs to dist/)
npm run build

# Preview production build locally
npm run preview

# Run ESLint to check code quality
npm run lint
```

## Technology Stack

- **Framework**: React 19.2.0
- **Build Tool**: Vite 7.2.4
- **Language**: JavaScript (JSX)
- **Linting**: ESLint 9 with flat config format
- **Fast Refresh**: Babel-based React plugin

## Project Structure

```
src/
├── App.jsx              # Main application component
├── pages/               # Page components
│   ├── Home.jsx
│   ├── About.jsx
│   └── Work.jsx
├── components/          # Reusable components
│   ├── Navbar.jsx
│   ├── Scene3D.jsx      # 3D scene rendering (planned)
│   └── Section.jsx
├── styles/              # CSS stylesheets
│   └── main.css
└── assets/              # Static assets
    ├── images/
    └── textures/        # 3D textures (planned)
```

Entry point: `/src/main.jsx` (referenced in `index.html`)

## ESLint Configuration

Uses the new flat config format (`eslint.config.js`). Custom rules:
- `no-unused-vars`: Allows unused variables with uppercase naming (constants/components)
- React Hooks and React Refresh rules enabled
- Targets ES2020+ with browser globals

## Architecture Notes

- The project follows a page-based routing structure with separate page components
- Appears to be designed for 3D content integration (Scene3D component, textures directory)
- Uses a component-based architecture typical of React applications
- No TypeScript - pure JavaScript with JSX
