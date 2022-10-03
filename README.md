# 🧰 Simple Puppeteer TypeScript Starter | 2022

This template will quickly help us build a project using Puppeteer and TypeScript for data scraping in public pages.

### Features

- Minimal
- TypeScript V4
- Testing with Jest
- Linting with Eslint and Prettier
- Local development with Nodemon
- IP Proxy

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
