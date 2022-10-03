# 🧰 Simple Puppeteer TypeScript Starter | 2022

> We talk about a lot of **advanced Node.js and TypeScript** concepts on [the blog](https://khalilstemmler.com), particularly focused around Domain-Driven Design and large-scale enterprise application patterns. However, I received a few emails from readers that were interested in seeing what a basic TypeScript starter project looks like. So I've put together just that.

### Features

- Minimal
- TypeScript v4
- Testing with Jest
- Linting with Eslint and Prettier
- Pre-commit hooks with Husky
- VS Code debugger scripts
- Local development with Nodemon

### Structure

```
  build
    └── index.js
    └── ...
  config
    └── config.json
  src
    └── pages
        ├── index.ts
        ├── identifiers.ts
        ├── userTemplate.ts
    └── environment
        ├── config.ts
    └── utils
        ├── index.ts
    └── index.ts
  types
    └── index.d.ts
```

### Scripts Overview

```NodeJS
npm run start:dev
```

Starts the application in development using nodemon and ts-node to do cold reloading.

```NodeJS
npm run build
```

Builds the app at build, cleaning the folder first.

```NodeJS
npm run start
```

Starts the app in production by first building the project with `npm run build`, and then executing the compiled JavaScript at `build/index.js`.
