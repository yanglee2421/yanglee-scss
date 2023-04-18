# yanglee-scss

## Installation

```powershell
# yarn
yarn add @yanglee2421/scss
# npm
npm i @yanglee2421/scss
```

## Quick Start

- vite.config.js

```js
// vite.config.js
import { ConfigEnv, defineConfig, UserConfig } from "vite";
import { resolve } from "node:path";

export default defineConfig((configEnv) => ({
  resolve: {
    alias: {
      "@": resolve(__dirname, "./src"),
    },
  },
  css: {
    preprocessorOptions: {
      scss: { additionalData: `@use "@yanglee2421/scss/src" as *;` },
    },
  },
}));
```

- main.js

```js
// Only load scss for reset
import "@yanglee2421/scss";
```
