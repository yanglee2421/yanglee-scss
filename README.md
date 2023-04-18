# yanglee-scss

![version](https://img.shields.io/badge/version-0.0.2-blue)
![npm](https://img.shields.io/badge/yan-v1.2.19-orange)
![dependencies](https://img.shields.io/badge/dependencies-scss-brightgreen)
![developer](https://img.shields.io/badge/developer-YangLee-f39f37)

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
import { defineConfig } from "vite";
import { resolve } from "node:path";

export default defineConfig((configEnv) => ({
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
