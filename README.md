# Reactesse Edge

> React + Vite + Edge Side Rendering template based on [@antfu](https://github.com/antfu)'s [Vitesse](https://github.com/antfu/vitesse) with [Vitedge](https://github.com/frandiox/vitedge).

<p align='center'>
<a href="https://reactesse.zable.workers.dev/">Live Demo</a>
</p>

## Features

- ⚡️ [React](https://github.com/facebook/react), [Vite 2](https://github.com/vitejs/vite), [ESBuild](https://github.com/evanw/esbuild)

- ⚔️ Edge-side rendering in Cloudflare Workers via [Vitedge](https://github.com/frandiox/vitedge), with edge cache and HTTP/2 server push

- 🗂 [File based routing](./src/pages)

- 🎨 [Windi CSS](https://github.com/windicss/windicss) - on-demand Tailwind CSS with speed

- 😃 [SVG icons](https://react-icons.github.io/react-icons/)

- 🌍 [I18n ready](./src/i18n/translations)

- 🗒 [Markdown Support](https://github.com/brillout/vite-plugin-mdx)

- 🦾 TypeScript, of course

- ☁️ Deploy on Cloudflare Workers, minimal [setup](./wrangler.toml)

<br>

## Pre-packed

### UI Frameworks

- [Windi CSS](https://github.com/windicss/windicss) (On-demand [TailwindCSS](https://tailwindcss.com/)) - lighter and faster, with a bundle additional features!
  - [Windi CSS Typography](https://windicss.netlify.app/guide/plugins.html#typography) - similar to [Tailwind CSS Typography](https://github.com/tailwindlabs/tailwindcss-typograph) but for Windi CSS

### Plugins

- [`vite-plugin-pages`](https://github.com/hannoeru/vite-plugin-pages) - file system based routing
- [`vite-plugin-windicss`](https://github.com/antfu/vite-plugin-windicss) - WindiCSS support
- [`vite-plugin-mdx`](https://github.com/brillout/vite-plugin-mdx) - Markdown as components / components in Markdown
- [`remark-prism`](https://github.com/sergioramos/remark-prism) - [Prism](https://prismjs.com/) for syntax highlighting
- [`prism-theme-vars`](https://github.com/antfu/prism-theme-vars) - customizable Prism.js theme using CSS variables
- [`react-i18next`](https://react.i18next.com/) - Internationalization
- [`react-helmet-async`](https://github.com/staylor/react-helmet-async) - manipulate document head reactively

### Dev tools

- [Vitedge](https://github.com/frandiox/vitedge) - Edge-side rendering
- [Miniflare](https://github.com/mrbbot/miniflare) - Preview your app in a worker environment locally
- [Wrangler](https://developers.cloudflare.com/workers/cli-wrangler/install-update) - Deploy to Cloudflare Workers
- [TypeScript](https://www.typescriptlang.org/)
- [VS Code Extensions](./.vscode/extensions.json)
  - [i18n Ally](https://marketplace.visualstudio.com/items?itemName=lokalise.i18n-ally)
  - [ESLint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint)

## Try it now!

### GitHub Template

[Create a repo from this template on GitHub](https://github.com/frandiox/reactesse-edge-template/generate).

### Clone to local

If you prefer to do it manually with the cleaner git history

```bash
npx degit frandiox/reactesse-edge-template my-reactesse-app
cd my-reactesse-app
npm i
```

## Checklist

When you use this template, try follow the checklist to update your info properly

- [ ] Add a `name` field in `package.json`
- [ ] Change the author name in `LICENSE`
- [ ] Change the favicon in `public`
- [ ] Remove the `.github` folder which contains the funding info
- [ ] Clean up the READMEs and remove routes

And, enjoy :)

## Usage

### Development

Just run and visit http://localhost:3333

```bash
npm run dev # SSR development
npm run dev:spa # SPA without SSR
```

### Build

To build the App, run

```bash
npm run build
```

And you will see the generated files in `dist`.

### Deploy on Cloudflare Workers

1. Create your [Cloudflare](https://www.cloudflare.com/) account.
2. Install [Wrangler](https://developers.cloudflare.com/workers/cli-wrangler/install-update) CLI.
3. Modify the `account_id` in [wrangler.toml](./worker-site/wrangler.toml). Then:

```bash
npm run preview # Simulate Worker environment locally
npm run deploy
```
