# astrojs-tailwind

A fork of the now-deprecated [@astrojs/tailwind](https://github.com/withastro/astro/tree/HEAD/packages/integrations/tailwind) integration, updated to support Astro v6. No other changes have been made.

## Installation
```sh
npm install @digital-zombie/astrojs-tailwind
pnpm add @digital-zombie/astrojs-tailwind
yarn add @digital-zombie/astrojs-tailwind
```

## Usage
```js
// astro.config.mjs
import { defineConfig } from "astro/config";
import tailwind from "@digital-zombie/astrojs-tailwind";

export default defineConfig({
  integrations: [tailwind()],
});
```

## Options

All options are identical to the original integration:

| Option | Type | Default | Description |
|---|---|---|---|
| `applyBaseStyles` | `boolean` | `true` | Inject Tailwind's base styles automatically |
| `configFile` | `string` | `undefined` | Path to a custom Tailwind config file |
| `nesting` | `boolean` | `false` | Enable `tailwindcss/nesting` plugin |

## Why does this exist?

`@astrojs/tailwind` was deprecated when Tailwind v4 launched and its maintainers dropped support for Astro v6. This fork exists for projects that want to stay on Tailwind v3 without migrating to the Vite plugin approach required by Tailwind v4.

## License

MIT

Copyright (c) 2023–present Astro contributors
