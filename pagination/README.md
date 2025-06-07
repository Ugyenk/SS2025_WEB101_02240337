# React + TypeScript + Vite

A simple template to get started with React, TypeScript, and Vite for fast development.

## What's Included

- React for building user interfaces
- TypeScript for type safety
- Vite for fast development and building
- ESLint for code quality

## Getting Started

1. Clone or create your project
2. Install dependencies: `npm install`
3. Start development server: `npm run dev`
4. Build for production: `npm run build`

## Available Plugins

You can choose between two React plugins:

- **@vitejs/plugin-react** - Uses Babel for Fast Refresh
- **@vitejs/plugin-react-swc** - Uses SWC for Fast Refresh (faster)

## Better Code Quality (Optional)

For production apps, you can add stricter ESLint rules:

```js
export default tseslint.config({
  extends: [
    ...tseslint.configs.recommendedTypeChecked,
    // or for even stricter rules:
    ...tseslint.configs.strictTypeChecked,
  ],
  languageOptions: {
    parserOptions: {
      project: ['./tsconfig.node.json', './tsconfig.app.json'],
      tsconfigRootDir: import.meta.dirname,
    },
  },
})
```

## React-Specific Linting

Add React-specific lint rules with these plugins:

```bash
npm install eslint-plugin-react-x eslint-plugin-react-dom
```

Then update your ESLint config:

```js
import reactX from 'eslint-plugin-react-x'
import reactDom from 'eslint-plugin-react-dom'

export default tseslint.config({
  plugins: {
    'react-x': reactX,
    'react-dom': reactDom,
  },
  rules: {
    ...reactX.configs['recommended-typescript'].rules,
    ...reactDom.configs.recommended.rules,
  },
})
```

## That's It

You're ready to start building with React, TypeScript, and Vite. Happy coding!